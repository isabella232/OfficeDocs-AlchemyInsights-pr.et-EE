---
title: Rakenduse tõrked
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "7841"
ms.openlocfilehash: ce4c89da79112726ed4fb25527edc8d082bd37f239595b9eab7279abeeecfd7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931445"
---
# <a name="application-errors"></a>Rakenduse tõrked

Kas otsite teavet **AADSTS-i** tõrkekoodide kohta, mis tagastatakse Azure Active Directory (Azure AD) turbelubade teenusest (STS)? AADSTS-i tõrkekirjelduste, paranduste ja mõne soovitatud lahenduse leidmiseks lugege [läbi Azure AD-autentimis-](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) ja autoriseerimistõrgete koodid.

Autoriseerimistõrked võivad tuleneda mitmest probleemist, millest enamik genereerib tõrkekoodi 401 või 403. Näiteks võivad autoriseerimistõrked olla järgmised.

- valed [pääsutõendi hankimisvood](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- kehvasti konfigureeritud [lubade ulatused](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- puuduv [nõusolek](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Levinumate autoriseerimistõrgete lahendamiseks proovige allpool toodud juhiseid, mis vastavad kõige paremini teile ilmnevale tõrkele. Võidakse kohaldada rohkem kui ühte.

**Tõrketeade „401 Puuduvad volitused“: kas teie tõend kehtib?**

Veenduge, et teie rakendus esitaks taotluse osana microsoft Graph kehtivat juurdepääsuluba. Sageli tähendab see tõrge, et pääsutõend on HTTP-autentimispäringu päisest puudu või et tõend on kehtetu või aegunud. Soovitame tungivalt kasutada microsofti [autentimisteegi (MSAL) juurdepääsulubade](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) omamiseks. Lisaks võib see tõrge ilmneda juhul, kui proovite kasutada isiklikule Microsofti kontole antud delegeeritud juurdepääsuluba, et pääseda juurde API-le, mis toetab ainult töö- või koolikontosid (organisatsioonikontosid).

**Tõrge „403 Keelatud“: kas olete valinud õige õiguste komplekti?**

Kontrollige, kas olete taotlenud õiget õiguste komplekti, võttes aluseks Microsoft Graph teie rakendusekõnede API-d. Soovitatavad vähima õigusega õigused on saadaval kõigis Microsoft Graph API viitemeetodi teemades. Lisaks peab kasutaja või administraator need õigused rakendusele andma. Õiguste andmine toimub tavaliselt nõusolekulehe kaudu või õiguste andmisel Azure'i portaali rakenduse registreerimise laba abil. Klõpsake rakenduse lehel **Settings** (Sätted) nuppu **Required Permissions** (Nõutavad õigused) ja seejärel nuppu **Grant Permissions** (Anna õigused).

- [Microsoft Graphi õigused](https://docs.microsoft.com/graph/permissions-reference) 
- [Azure AD pääsuõiguste ja nõusoleku mõistmine](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**Tõrge „403 Keelatud“: kas teie rakendus hankis valitud pääsuõigustele vastava tõendi?**

Veenduge, et taotletud või antud õiguste tüüp vastaks teie rakenduse hangitud juurdepääsulubade tüübile. Võimalik, et taotlete ja annate rakendusele õigusi, kuid kasutate kliendi identimisteabe voo märkide asemel delegeeritud interaktiivse koodivoo tõendeid või taotlete ja annate delegeeritud õigusi, kuid kasutate delegeeritud koodivoo märkide asemel kliendi identimisteabevoo tõendeid.

- [Kasutajate nimel juurdepääsu saamine ja delegeeritud pääsuõigused](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v2.0 – OAuth 2.0 autoriseerimiskoodi voog](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Juurdepääsu saamine ilma kasutajata (deemoniteenus) ja rakenduseõigused](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v2.0 – OAuth 2.0 kliendi identimisteabe voog](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**Tõrge „403 Keelatud“: parooli lähtestamine**

Praegu pole selliseid rakenduseõiguste deemoni teenustevahelisi õigusi, mis lubaksid kasutajate paroole lähtestada. Need API-d on toetatud üksnes sisselogitud administraatoriga interaktiivse delegeeritud koodi voogude kasutamisel.

- [Microsoft Graphi õigused](https://docs.microsoft.com/graph/permissions-reference)

**Tõrge „403 Keelatud“: kas kasutajal on juurdepääs ja litsents?**

Delegeeritud koodivoogude korral hindab Microsoft Graph, kas taotlus on lubatud rakendusele antud õiguste ja sisse logitud kasutaja õiguste põhjal. Üldiselt tähendab see tõrkekood, et kasutajal pole päringu jaoks piisavaid õigusi või kasutajal pole juurdepääsetavate andmete jaoks litsentsi. Päringu saavad edukalt teha ainult nõutavate pääsuõiguste või litsentsidega kasutajad.

**Tõrge „403 Keelatud“: kas valisite õige ressursi API?**

API-teenused (nt Microsoft Graph) kontrollige, kas saadud juurdepääsuluba helinõue (publikule) vastab väärtusele, mida ta enda jaoks eeldab, ja kui ei, siis kuvatakse tõrge 403 Keelatud. Üks levinud viga, mis selle tõrke põhjustab, on katse kasutada Azure AD Graphi API-sid, Outlooki API-sid või SharePointi/OneDrive‘i API-sid Microsoft Graphi kutsumiseks (või vastupidi). Veenduge, et ressurss (või ulatus), mille jaoks teie rakendus tõendi hangib, vastaks API-le, mida rakendus kutsub.

**Tõrge „400 Vigane päring“ või „403 Keelatud“: kas kasutaja järgib oma asutuse või ettevõtte tingimuspääsu poliitikaid?**

Ettevõtte CA-poliitikate põhjal võidakse teie rakenduse kaudu Microsoft Graph ressurssidele juurdepääsev kasutaja esitada väljakutse lisateabe saamiseks, mida teie rakenduse algselt hangitud juurdepääsuluba ei esitata. Sel juhul saab teie rakendus pääsutõendi hankimisel tõrkekoodi 400 *interaction_required* („400: vaja on suhtlust“) või Microsoft Graphi kutsumisel tõrkekoodi 403 *insufficient_claims* („403: ebapiisavad väited“). Mõlemal juhul sisaldab tõrkevastus lisateavet, mida saab esitada lõpp-punktile, et kasutajat lisateabe saamiseks (nt mitmikautentimist või seadme registreerimist) esitada.

- [Tingimusjuurdepääsu probleemide lahendamine MSAL-i abil ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Arendusjuhised Azure Active Directory tingimuspääsu jaoks](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
