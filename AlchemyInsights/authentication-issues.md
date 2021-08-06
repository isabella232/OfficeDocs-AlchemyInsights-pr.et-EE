---
title: Autentimisprobleemid
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: c7e6d96940f8d7052ee4b49b22c0d1d7d5bd5f9277f4a7eff709def1da2e13af
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019504"
---
# <a name="authentication-issues"></a>Autentimisprobleemid

**Kas otsite teavet Azure Active Directory (Azure AD) turbetõenditeenuse (STS) tagastatavate AADSTS-i tõrkekoodide kohta?** AADSTS-i tõrgete kirjeldused, lahendused ja soovitatavad ajutised lahendused leiate artiklist [Azure AD autentimise ja autoriseerimise tõrkekoodid](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes).

Autoriseerimistõrked võivad tuleneda mitmest probleemist, millest enamik genereerib tõrkekoodi 401 või 403. Autoriseerimistõrgeteni võivad viia näiteks kõik järgmised probleemid:

- valed [pääsutõendi hankimisvood](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- kehvasti konfigureeritud [lubade ulatused](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- puuduv [nõusolek](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Levinud autoriseerimistõrgete kõrvaldamiseks proovige allpool kirjeldatud lahenduskäike, mis vastavad teie tõrkele kõige täpsemini. Teie tõrketeatele võib vastata mitu lahenduskäiku.

**Tõrketeade „401 Puuduvad volitused“: kas teie tõend kehtib?**

Veenduge, et teie rakendus esitaks päringu raames Microsoft Graphile kehtiva pääsutõendi. Sageli tähendab see tõrge, et pääsutõend on HTTP-autentimispäringu päisest puudu või et tõend on kehtetu või aegunud. Soovitame teil pääsutõendite hankimiseks kasutada Microsofti autentimisteeki (Microsoft Authentication Library – MSAL). Lisaks võib see tõrge ilmneda juhul, kui proovite kasutada isiklikule Microsofti kontole antud delegeeritud pääsutõendit juurdepääsuks API-le, mis toetab ainult töö- või koolikontosid (organisatsioonikontosid).

**Tõrge „403 Keelatud“: kas olete valinud õige õiguste komplekti?**

Veenduge, et olete taotlenud õiget pääsuõiguste komplekti lähtuvalt teie rakenduse kutsutavatest Microsoft Graphi API-dest. Soovitatavad minimaalõigused on ära toodud kõigis Microsoft Graphi API viitemeetodi artiklites. Lisaks peab kasutaja või administraator need õigused rakendusele andma. Õiguste andmine toimub tavaliselt nõusolekulehe või Azure‘i portaali rakenduseregistreerimise serverilehe kaudu. Klõpsake rakenduse lehel **Settings** (Sätted) nuppu **Required Permissions** (Nõutavad õigused) ja seejärel nuppu **Grant Permissions** (Anna õigused). Lisateavet leiate järgmistest teemadest:

- [Microsoft Graphi õigused](https://docs.microsoft.com/graph/permissions-reference) 
- [Azure AD pääsuõiguste ja nõusoleku mõistmine](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**Tõrge „403 Keelatud“: kas teie rakendus hankis valitud pääsuõigustele vastava tõendi?**

Veenduge, et taotletud või antud pääsuõiguste tüübid vastaksid teie rakenduse hangitava pääsutõendi tüübile. On võimalik, et taotlete ja annate rakenduseõigusi, ent kasutate kliendi identimisteabe voo tõendite asemel delegeeritud interaktiivse koodi voo tõendeid või taotlete ja annate delegeeritud õigusi, ent kasutate delegeeritud koodi voo tõendite asemel kliendi identimisteabe voo tõendeid.

Tõendite hankimise kohta leiate lisateavet järgmistest teemadest:

- [Kasutajate nimel juurdepääsu saamine ja delegeeritud pääsuõigused](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v2.0 – OAuth 2.0 autoriseerimiskoodi voog](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Juurdepääsu saamine ilma kasutajata (deemoniteenus) ja rakenduseõigused](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v2.0 – OAuth 2.0 kliendi identimisteabe voog](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**Tõrge „403 Keelatud“: parooli lähtestamine**

Praegu pole selliseid rakenduseõiguste deemoni teenustevahelisi õigusi, mis lubaksid kasutajate paroole lähtestada. Need API-d on toetatud üksnes sisselogitud administraatoriga interaktiivse delegeeritud koodi voogude kasutamisel. Lisateavet leiate artiklist [Microsoft Graphi õigused](https://docs.microsoft.com/graph/permissions-reference).

**Tõrge „403 Keelatud“: kas kasutajal on juurdepääs ja litsents?**

Delegeeritud koodi voogude korral hindab Microsoft Graph, kas päring on lubatud, võttes aluseks rakendusele antud pääsuõigused ja sisselogitud kasutaja pääsuõigused. Üldiselt tähendab see tõrkekood, et kasutajal pole päringu jaoks piisavaid õigusi **või** kasutajal pole juurdepääsetavate andmete jaoks litsentsi. Päringu saavad edukalt teha ainult nõutavate pääsuõiguste või litsentsidega kasutajad.

**Tõrge „403 Keelatud“: kas valisite õige ressursi API?**

API-teenused, näiteks Microsoft Graph, kontrollivad, kas saadud pääsutõendi väide *aud* (järgijaskond) vastab eeldatud väärtusele; kui ei vasta, ilmnebki tõrge „403 Keelatud“. Üks levinud viga, mis selle tõrke põhjustab, on katse kasutada Azure AD Graphi API-sid, Outlooki API-sid või SharePointi/OneDrive‘i API-sid Microsoft Graphi kutsumiseks (või vastupidi). Veenduge, et ressurss (või ulatus), mille jaoks teie rakendus tõendi hangib, vastaks API-le, mida rakendus kutsub.

**Tõrge „400 Vigane päring“ või „403 Keelatud“: kas kasutaja järgib oma asutuse või ettevõtte tingimuspääsu poliitikaid?**

Lähtuvalt asutuse või ettevõtte tingimuspääsu poliitikatest võidakse kasutajalt, kes proovib teie rakenduse kaudu pääseda juurde Microsoft Graphi ressurssidele, küsida lisateavet, mida teie rakenduse algselt hangitud pääsutõendis ei ole. Sel juhul saab teie rakendus pääsutõendi hankimisel tõrkekoodi **400 *interaction_required*** („400: vaja on suhtlust“) või Microsoft Graphi kutsumisel tõrkekoodi **403 *insufficient_claims*** („403: ebapiisavad väited“). Kummalgi juhul sisaldab tõrkevastus lisateavet, mille saab volitatud lõpp-punktile esitada kasutajalt lisateabe küsimiseks (nt mitmikautentimine või seadme registreerimine).

Tingimuspääsu kohta leiate lisateavet järgmistest artiklitest:

- [Tingimuspääsu pretensioonide käitlemine MSAL-i kaudu](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Arendusjuhised Azure Active Directory tingimuspääsu jaoks](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

***Autentimisteegi (ADAL) Azure Active Directory Azure AD Graph API (AAD Graph) tugi***

- Alates 30. juunist 2020 ei lisa me enam uusi funktsioone Azure Active Directory autentimisteeki (ADAL) ja Azure AD Graphi API-sse (AAD Graphi). Pakume endiselt tehnilist tuge ja turbevärskendusi, ent mitte enam funktsioonivärskendusi.
- Alates 30. juunist 2022 lõpetame ADAL-i ja AAD Graphi tootetoe ega paku enam tehnilist tuge ega turbevärskendusi.
    - Olemasolevates opsüsteemiversioonides ADAL-i kasutavad rakendused töötavad edasi ka pärast seda, ent ei saa enam tehnilist tuge ega turbevärskendusi.
    - AAD Graphi kasutavad rakendused ei pruugi pärast seda enam AAD Graphi lõpp-punktist vastuseid saada.

**ADAL-migreerimine**

Soovitame võtta kasutusele [Microsofti autentimisteegi (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), mis sisaldab uusimaid funktsioone ja turbevärskendusi. Soovituse kontekst on Microsofti otsus migreerida oma rakendused tootetoe lõpptähtajaks MSAL-i. Microsofti rakenduste MSAL-i migreerimise eesmärk on tagada, et rakendused saaksid kasu MSAL-i jätkuvatest turbe- ja funktsioonitäiustustest.

- [Lugege ADAL-i KKK-d.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Lugege lisateavet rakenduste platvormipõhise migreerimise kohta.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Kui te pole kindel, millised teie rakendused kasutavad ADAL-i, soovitame teil vaadata kõigi oma rakenduste lähtekoodi. Kui vaja, võtke ühendust asjakohaste sõltumatute tarkvaratootjate (ISV-de) või rakendusepakkujatega. Samuti saab Microsofti tugi anda teile nimekirja kõigist neist mitte-Microsofti rakendustest teie rentnikkeskkonnas, mis kasutavad ADAL-i.

**AAD Graphi migreerimine**

AAD Graphi kasutavate rakenduste korral täitke meie juhtnöörid [Azure AD Graphi rakenduste migreerimiseks Microsoft Graphi](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Meie migreerimise kontroll-loend on hea koht alustamiseks](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- Azure‘i rakenduste registreerimisportaalis näete, millised rakendused kasutavad AAD Graphi. Soovitame teil kõigi rakenduste lähtekood läbi vaadata ja kui vaja, võtta ühendust ISV-de või rakendusepakkujatega. Lisaks võib ka Microsofti tugi anda teile teavet AAD Graphi kasutuse kohta teie rentnikkeskkonnas.

 










