---
title: Microsoft Graph API probleemid
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "7759"
ms.openlocfilehash: 9df021211c8a65997889d9303dbf28a27104cfa95841d4cb810427c652ba0784
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975889"
---
# <a name="microsoft-graph-api-issues"></a>Microsoft Graph API probleemid

See teema võib kehtida ka arendajatele, kes kasutavad endiselt Azure AD Graph API-d. Siiski on tungivalt **soovitatav** kasutada Microsoft Graph kõiki oma kataloogi-, identiteedi- ja juurdepääsuhalduse stsenaariume.

**Autentimis- või autoriseerimisprobleemid**

- Kui teie rakendus ei **saa** microsoft Graph'ile helistamiseks tõendeid hankida, valige selle teema kohta konkreetsema spikri ja toe saamiseks probleem microsoft Graph-kategooria juurdepääsulubade **(autentimine)** kasutamisel.
- Kui teie rakendus saab Microsoft Graph'ile helistamisel **401 või 403** autoriseerimistõrkeid, valige selle teema kohta lisateabe saamiseks kategooria Juurdepääsu keelamine **(autoriseerimine)** Microsoft Graph API.

**Soovin kasutada Microsoft Graph, kuid pole kindel, kust alustada**

- [Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Microsoft Graph rakenduste loomise alustamine](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – Microsoft Graph API-de testimine rentniku rentnikus või demo rentnikus

**Soovin kasutada Microsoft Graph, kuid kas see toetab v1.0 kataloogi API-sid, mida vajan?**

Microsoft Graph on soovitatav API kataloogi-, identiteedi- ja juurdepääsuhalduse jaoks. Siiski on Azure AD-d ja Microsoft Graph vahel veel Graph. Vaadake üle järgmised artiklid, mis tõstavad esile kõige aja ajasemad erinevused, mis aitavad teil valida.

- [Ressursitüübi erinevused Azure AD Graph Ja Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Azure AD Graph Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Azure AD ja Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Helistav API ei tööta – kus saab teha rohkem testimist?**

**Microsoft Graph Explorer** – microsoft Graph API-sid oma rentnikus või demo  rentnikus ning tutvuge microsoft Graph Exploreri näidispäringutega.

**Minu rakendus on liiga aeglane ja aheneb ka. Milliseid täiustusi saan teha?**

Olenevalt teie stsenaariumist on teie käsutuses mitmesuguseid võimalusi, mis muudavad teie rakenduse rohkem esinejaks ja mõnel juhul on teenuse ahendamise võimalus väiksem (kui teete liiga palju kõnesid).

- [Microsoft Graph head tavad](https://docs.microsoft.com/graph/best-practices-concept)
- [Pakketaotlused](https://docs.microsoft.com/graph/json-batching)
- [Muutuste jälitamine deltapäringu kaudu](https://docs.microsoft.com/graph/delta-query-overview)
- [Muudatustest teavitatakse veebihoobide kaudu](https://docs.microsoft.com/graph/webhooks)
- [Ahendamise juhised](https://docs.microsoft.com/graph/throttling)

**Kust leida lisateavet tõrgete ja teadaolevate probleemide kohta?**

- [Microsoft Graph tõrkevastuse teave](https://docs.microsoft.com/graph/errors)
- [Teadaolevad microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Kus saab kontrollida teenuse kättesaadavuse ja ühenduvuse olekut?**

Microsoft Graph kaudu juurdepääsetud teenuste kättesaadavus ja ühenduvus võivad mõjutada Microsofti teenuste üldist kättesaadavust ja Graph.

- Teenuse Azure Active Directory seisundi tagamiseks kontrollige Azure'i olekulehel loetletud turbe- ja [identiteediteenuste olekut.](https://azure.microsoft.com/status/) 
- Kui Office microsoft Graph, kontrollige teenuse seisundi [armatuurlaual Office teenuste olekut.](https://portal.office.com/adminportal/home#/servicehealth)

Microsoft Graph autoriseerimistõrked võivad tuleneda mitmest erinevast probleemist, millest enamik genereerib tõrke 401 või 403. Näiteks võivad autoriseerimistõrked olla järgmised.

- valed [pääsutõendi hankimisvood](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- kehvasti konfigureeritud [lubade ulatused](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- puuduv [nõusolek](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

***Autentimisteegi (ADAL) Azure Active Directory Azure AD Graph API (AAD Graph) tugi***

**Alates 30. juunist 2020** ei lisa me enam ADAL-i ja Azure AD Graph. Pakume endiselt tehnilist tuge ja turbevärskendusi, ent mitte enam funktsioonivärskendusi.

**Alates 30. juunist 2022** lõpetame ADAL ja Azure AD Graph ning ei paku enam tehnilist tuge ega turbevärskendusi.

Rakendused, mis kasutavad ADAL-i olemasolevate operatsioonisüsteemi versioonide korral, töötavad ka edaspidi, kuid ei *saa tehnilist tuge ega turbevärskendusi.*

Rakendused, mis kasutavad Azure AD Graph i pärast seda aega, ei pruugi enam azure AD-Graph vastuseid saada.

**ADAL-migreerimine**

Soovitame võtta kasutusele [Microsofti autentimisteegi (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), mis sisaldab uusimaid funktsioone ja turbevärskendusi.

Kui kasutate Microsofti rakendusi, siis tea, et Microsoft migreerib oma rakendused MSAL-i toe lõpu tähtajaks, tagades neile MSAL-i jätkuva turbe- ja funktsioonitäiustuste kasutamise.

1. [Lugege ADAL-i KKK-d.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Lugege lisateavet rakenduste platvormipõhise migreerimise kohta.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Kui vajate abi selle mõistmisel, milline teie rakendustest ADAL-i kasutab, soovitame teil läbi vaadata kõik rakenduste lähtekoodid ja vajaduse korral ühendust võtta mis tahes ISV-dega või rakendusepakkujatega. Samuti saab Microsofti tugi anda teile nimekirja kõigist neist mitte-Microsofti rakendustest teie rentnikkeskkonnas, mis kasutavad ADAL-i.

**AAD Graphi migreerimine**

Azure AD-d Graph rakenduste puhul järgige meie juhiseid [Azure AD Graph microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Meie migreerimise kontroll-loend on hea koht alustamiseks](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Azure‘i rakenduste registreerimisportaalis näete, millised rakendused kasutavad AAD Graphi. Soovitame teil kõigi rakenduste lähtekood läbi vaadata ja kui vaja, võtta ühendust ISV-de või rakendusepakkujatega. Microsofti tugiteenuste abil saate ka vaadata kõiki AAD-Graph kasutust.
3. Selleks et teie rakendus pääseks microsoft Graph andmetele juurde, peab kasutaja või administraator andma sellele nõusolekuprotsessi kaudu õiged õigused. Microsofti [Graph õiguste viites](https://docs.microsoft.com/graph/permissions-reference) on loetletud kõigi Microsoft Graph API-dega seotud õigused. Samuti annab see juhiseid õiguste kasutamise kohta.
