---
title: Autentimisteekidega seotud probleemid
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
- "9004333"
- "7731"
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028000"
---
# <a name="issues-with-authentication-libraries"></a>Autentimisteekidega seotud probleemid

1. [Microsofti identimisplatvorm autentimisteekides](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) on loetletud Microsofti toetatud ja ühilduvad kliendi- ja vahetööteegid.
2. Microsofti autentimisteek (MSAL) toetab mitut [autentimisvoogu,](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) mida saab kasutada erinevates rakendusestsenaariumites.
3. Märkide autentimiseks ja omandamiseks lähtestage uus avalik või konfidentsiaalne klientrakendus oma koodis. Kliendirakenduse lähtestamisel Microsofti autentimisteegis (MSAL) saate määrata mitu konfigureerimissuvandeid. Lisateavet leiate teemast Rakenduse [konfiguratsioonisuvandid.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)

**Autentimisteegi (ADAL) Azure Active Directory Azure AD Graph API (AAD Graph) tugi**

**Alates 30. juunist 2020** ei lisa me enam ADAL-i ja Azure AD Graph. Pakume endiselt tehnilist tuge ja turbevärskendusi, ent mitte enam funktsioonivärskendusi.

**Alates 30. juunist 2022** lõpetame ADAL ja Azure AD Graph ning ei paku enam tehnilist tuge ega turbevärskendusi.

Rakendused, mis kasutavad ADAL-i olemasolevate operatsioonisüsteemi versioonide korral, töötavad ka edaspidi, kuid ei *saa tehnilist tuge ega turbevärskendusi.*

Rakendused, mis kasutavad Azure AD Graph i pärast seda aega, ei pruugi enam azure AD-Graph vastuseid saada.

**ADAL-migreerimine**

Soovitame võtta kasutusele [Microsofti autentimisteegi (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), mis sisaldab uusimaid funktsioone ja turbevärskendusi.

Kui kasutate Microsofti rakendusi, siis tea, et Microsoft migreerib oma rakendused MSAL-i tugiteenuste tähtajaks, tagades neile MSAL-i jätkuva turbe- ja funktsioonitäiustuste kasutamise.

Lisateavet leiate järgmistest teemadest.

1. [Lugege ADAL-i KKK-d.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Lugege lisateavet rakenduste platvormipõhise migreerimise kohta.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Kui vajate abi selle mõistmisel, milline teie rakendustest ADAL-i kasutab, soovitame teil läbi vaadata kõik rakenduste lähtekoodid ja vajaduse korral ühendust võtta mis tahes ISV-dega või rakendusepakkujatega. Samuti saab Microsofti tugi anda teile nimekirja kõigist neist mitte-Microsofti rakendustest teie rentnikkeskkonnas, mis kasutavad ADAL-i.

**AAD Graphi migreerimine**

Azure AD-d Graph rakenduste puhul järgige meie juhiseid [Azure AD Graph microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Meie migreerimise kontroll-loend pakub alustamispunkti.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Azure‘i rakenduste registreerimisportaalis näete, millised rakendused kasutavad AAD Graphi. Soovitame teil kõigi rakenduste lähtekood läbi vaadata ja kui vaja, võtta ühendust ISV-de või rakendusepakkujatega. Microsofti tugiteenuste abil saate ka vaadata kõiki AAD-Graph kasutust.
3. Selleks et teie rakendus pääseks microsoft Graph andmetele juurde, peab kasutaja või administraator andma sellele nõusolekuprotsessi kaudu õiged õigused. Microsofti [Graph õiguste viites](https://docs.microsoft.com/graph/permissions-reference) on loetletud kõigi Microsoft Graph API-dega seotud õigused. Samuti annab see juhiseid õiguste kasutamise kohta.
