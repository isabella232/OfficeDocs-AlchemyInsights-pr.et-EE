---
title: API-de rakenduste arendamisega seotud probleemid
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
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974381"
---
# <a name="issues-developing-applications-with-apis"></a>API-de rakenduste arendamisega seotud probleemid

Azure Active Directory graafiku API kasutamise alustamiseks lugege artiklit [AZURE ad Graph API Kiirjuhend juhend](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) või vaadake [interaktiivset AZURE ad Graph API dokumentatsiooni](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).

**Azure Active Directory autentimise teegi (ADAL) ja Azure AD Graphi API (AAD Graph) toe lõppemine**

**Alates 30 juunist 2020** ei lisa me enam ADAL ja Azure AD Graphi uusi funktsioone. Jätkame tehnilise toe ja turvavärskenduste esitamist, kuid ei paku enam funktsioonide värskendusi.

**Alates 30 juuni 2022**, lõpetame ADAL ja Azure AD Graphi toe ning ei paku enam tehnilist tuge ega turvavärskendusi.

Rakendused, mis kasutavad ADAL olemasolevatel OPERATSIOONISÜSTEEMI versioonidel, jätkavad tööd ka pärast seda, kuid ei saa tehnilist tuge ega turvavärskendusi.

Azure AD Graphi rakendused ei pruugi pärast selle aja möödumist enam saada vastuseid Azure AD Graphi lõpp-punktist.

**ADAL migreerimine**

Soovitame värskendada [Microsoft Authenticationi teeki (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), millel on uusimad funktsioonid ja turvavärskendused.

Kui kasutate Microsoft apps ' i, saate teada, et Microsoft on oma rakenduste migreerimise protsessis MSAL lõpptähtajaks, tagades, et nad saavad kasu MSAL pidevast turbest ja funktsioonide täiustustest.

1. [Lugege ADAL KKK-sid](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [Siit saate teada, kuidas rakendusi ühe platvormi põhjal migreerida](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. Kui vajate abi selle mõistmiseks, mida teie rakendused kasutavad ADAL, soovitame teil kõigi rakenduste lähtekoodi üle vaadata ja vajadusel jõuda kõigi tarkvaratoode või rakenduste pakkujatega. Microsofti tugiteenused võivad anda teile ka kõigi teie rentniku jaoks mitte-Microsofti ADAL rakenduste loendi.

**AAD Graphi migreerimine**

Rakendusi, mis kasutavad Azure AD Graphi, järgige meie juhiseid [AZURE ad Graphi rakenduste migreerimiseks Microsoft Graphi](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).

1. [Meie migreerimise kontroll-loend on](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)alustamine. 
1. Teie Azure ' i rakenduse registreerimise portaal näitab, millised rakendused kasutavad AAD graafikut. Soovitame üle vaadata kõik rakenduste lähtekoodi ja vajaduse korral jõuda mõnele tarkvaratoode või rakenduste pakkujale. Microsofti tugiteenused võivad teile pakkuda ka teie rentniku kõigi AAD Graphide kasutuse loendit.
1. Rakenduses Microsoft Graph andmetele juurdepääsemiseks peab kasutaja või administraator andma sellele loa andmiseks õiged õigused. [Microsoft Graph permissions References](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) loetletakse kõigi Microsoft Graphi API-de põhikomplektiga seotud load. See sisaldab ka juhiseid selle kohta, kuidas kasutada lube.
