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
ms.openlocfilehash: 2ef90b54ce222a06740e05891fabe87b6565cb14
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/25/2021
ms.locfileid: "49984540"
---
# <a name="application-errors"></a>Rakenduse tõrked

Kas otsite teavet Azure Active Directory (Azure AD) turbelubade teenusest (STS) tagastatud **AADSTS tõrkekoodidest** ? Lugege [AZURE ad autentimine ja autoriseerimise tõrkekoodid](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) , et leida AADSTS, parandusi ja muid soovitatud lahendusi.

Autoriseerimise tõrked võivad olla tingitud mitmest erinevast probleemist, millest enamik tekitab 401 või 403 tõrke. Näiteks võib järgmine tõrketeade olla järgmine:

- Ebaõiged juurdepääsuluba [omandavad vood](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- Halvasti konfigureeritud [õiguste ulatused](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- [Nõusoleku](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent) puudumine

Levinud autoriseerimise tõrgete lahendamiseks proovige allpool toodud juhiseid, mis vastavad kõige sagedamini teie saadud tõrkele. Rakendada võib ka rohkem kui ühte.

**401 lubamatu tõrge: kas teie luba kehtib?**

Veenduge, et teie rakendus esitaks taotluse osana Microsoft Graphi kehtiva juurdepääsuluba. See tõrge tähendab sageli, et juurdepääsuluba võib olla puudu HTTP autentimine taotluse päises või et see on kehtetu või aegunud. Soovitame kasutada Accessi turbelubade omandamiseks [Microsofti autentimise teeki (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) . See tõrge võib ilmneda juhul, kui proovite kasutada isiklikule Microsofti kontole antud volitatud juurdepääsuluba, et pääseda juurde API-ile, mis toetab ainult töö-või kooli kontosid (organisatsioonilised kontod).

**403 keelatud tõrge: Kas olete valinud õige õiguste kogumi?**

Veenduge, et olete taotlenud rakenduse Microsoft Graph API-l põhinevaid õigeid kasutajaõigusi. Soovitatavad kõige vähem privilegeeritud õigused on saadaval kõigis Microsoft Graphi API standardmeetodites. Lisaks sellele peab kasutaja või administraator need õigused andma. Õiguse andmine toimub tavaliselt nõusoleku lehe kaudu või lubade andmisega Azure ' i portaali rakenduse registreerimiskood abil. Klõpsake rakenduse **sätete** Blade nuppu **nõutavad load** ja seejärel käsku **Anna õigustele**.

- [Microsoft Graphi load](https://docs.microsoft.com/graph/permissions-reference) 
- [Azure AD kasutajaõiguste ja nõusoleku mõistmine](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 keelatud tõrge: kas teie rakendus omandas tõendi valitud õigustele vastamiseks?**

Veenduge, et taotletud või antud õiguse tüüp vastab teie rakenduse omandatava juurdepääsuloa tüübile. Võib-olla taotlete ja lubate rakenduse kasutusõigusi, kuid kasutate delegeeritud interaktiivse koodi voo märkide asemel kliendi mandaatide voogude märke või taotlete ja andes delegeeritud õiguseid, kuid kasutavad delegeeritud koodi voo asemel kliendi mandaatide voogude märke.

- [Juurdepääsu saamine kasutajate nimel ja delegeeritud õigustest](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v 2.0-OAuthi 2,0 loa koodi voog](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Juurdepääsu saamine kasutajata (Daemon Service) ja rakenduse kasutusõigused](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v 2.0-OAuthi 2,0 kliendi mandaatide voog](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 keelatud tõrge: parooli ennistamine**

Praegu ei ole rakenduse luba Daemon Service-to-teenuse õigusi, mis lubavad kasutaja paroole uuesti määrata. Neid API-sid toetatakse ainult interaktiivse delegeeritud koodi abil, millel on sisse logitud administraator.

- [Microsoft Graphi load](https://docs.microsoft.com/graph/permissions-reference)

**403 keelatud: kas kasutajal on juurdepääs ja need on litsentsitud?**

Delegeeritud koodi voogude korral hindab Microsoft Graph, kas taotlus on lubatud vastavalt rakenduse antud õigustele ja sisselogitud kasutaja õigustele. Üldiselt näitab see tõrge, et kasutajal pole piisavalt õigusi taotluse tegemiseks või kui kasutaja ei ole litsentsitud andmetele juurdepääsetav. Taotlust saab edukalt teha ainult selliste kasutajatega, kellel on nõutavad load või litsentsid.

**403 keelatud: kas valisite õige ressursi API?**

API-teenused (nt Microsoft Graph) kontrollivad, et saadud juurdepääsuluba (sihtrühm) vastab väärtusele, mida ta endale ootab, ja kui ei, siis tulemuseks on 403 keelatud tõrge. Sellest tõrkest tulenev levinud viga proovib kasutada Azure AD Graph API-de, Outlooki API-de või SharePointi/OneDrive ' i API-de jaoks saadud tõendit, et helistada Microsoft Graphile (või vastupidi). Veenduge, et teie rakenduse ressurss (või rakendusala) omandaks tõendi selle kohta, mis vastab rakenduse jaoks kasutatavale API-ile.

**400 halb taotlus või 403 keelatud: kas kasutaja täidab oma asutuse tingimusjuurdepääsu (CA) poliitika?**

Asutuse CA-i poliitika põhjal võidakse rakenduses Microsoft Graph ressurssidele juurdepääsuks teie rakenduse kaudu vaidlustada lisateavet, mida teie rakendus algselt soetatud juurdepääsuluba ei kasuta. Sellisel juhul saab teie rakendus 400, millel on *interaction_required* tõrge Accessi turbelubade omandamise ajal või 403, kus on Microsoft Graphi helistamisel *insufficient_claims* tõrge. Mõlemal juhul sisaldab tõrketeade lisateavet, mida saab autoriseerimise lõpp-punktina esitada, et esitada kasutajale lisateavet (nt mitme teguri autentimine või seadme registreerimine).

- [MSAL abil tingimusjuurdepääsu probleemide käsitlemine ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Azure Active Directory rakenduse arendaja juhised tingimusjuurdepääsu jaoks](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
