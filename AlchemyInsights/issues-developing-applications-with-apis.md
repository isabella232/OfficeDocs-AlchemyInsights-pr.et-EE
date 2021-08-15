---
title: API-ga rakenduste arendamisega seotud probleemid
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
- "9004343"
- "7755"
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013456"
---
# <a name="issues-developing-applications-with-apis"></a>API-ga rakenduste arendamisega seotud probleemid

Azure Active Directory Graph API kasutamise alustamiseks lugege Azure [AD Graph API lühijuhendit](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) või vaadake [interaktiivset Azure AD Graph API viitedokumenti.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)

**Autentimisteegi (ADAL) Azure Active Directory Azure AD Graph API (AAD Graph) tugi**

**Alates 30. juunist 2020** ei lisa me enam ADAL-i ja Azure AD Graph. Pakume endiselt tehnilist tuge ja turbevärskendusi, ent mitte enam funktsioonivärskendusi.

**Alates 30. juunist 2022** lõpetame ADAL ja Azure AD Graph ning ei paku enam tehnilist tuge ega turbevärskendusi.

Olemasolevates opsüsteemiversioonides ADAL-i kasutavad rakendused töötavad edasi ka pärast seda, ent ei saa enam tehnilist tuge ega turbevärskendusi.

Rakendused, mis kasutavad Azure AD Graph i pärast seda aega, ei pruugi enam azure AD-Graph vastuseid saada.

**ADAL-migreerimine**

Soovitame võtta kasutusele [Microsofti autentimisteegi (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), mis sisaldab uusimaid funktsioone ja turbevärskendusi.

Kui kasutate Microsofti rakendusi, siis tea, et Microsoft migreerib oma rakendused MSAL-i tugiteenuste tähtajaks, tagades neile MSAL-i jätkuva turbe- ja funktsioonitäiustuste kasutamise.

1. [Lugege läbi ADAL-i KKK.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. [Siit saate teada, kuidas migreerida rakendusi platvormipõhiselt.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. Kui vajate abi selle mõistmisel, milline teie rakendustest ADAL-i kasutab, soovitame teil läbi vaadata kõik rakenduste lähtekoodid ja vajaduse korral ühendust võtta mis tahes ISV-dega või rakendusepakkujatega. Samuti saab Microsofti tugi anda teile nimekirja kõigist neist mitte-Microsofti rakendustest teie rentnikkeskkonnas, mis kasutavad ADAL-i.

**AAD Graphi migreerimine**

Azure AD-d Graph rakenduste puhul järgige meie juhiseid [Azure AD Graph microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)

1. [Meie migreerimise kontroll-loend on hea koht alustamiseks](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Azure‘i rakenduste registreerimisportaalis näete, millised rakendused kasutavad AAD Graphi. Soovitame teil kõigi rakenduste lähtekood läbi vaadata ja kui vaja, võtta ühendust ISV-de või rakendusepakkujatega. Microsofti tugiteenuste abil saate ka vaadata kõiki AAD-Graph kasutust.
1. Selleks et teie rakendus pääseks microsoft Graph andmetele juurde, peab kasutaja või administraator andma sellele nõusolekuprotsessi kaudu õiged õigused. Microsofti [Graph õiguste viites](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) on loetletud kõigi Microsoft Graph API-dega seotud õigused. Samuti annab see juhiseid õiguste kasutamise kohta.
