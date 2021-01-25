---
title: Rakenduste väljatöötamise probleemid
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
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974304"
---
# <a name="issues-developing-applications"></a>Rakenduste väljatöötamise probleemid

Azure Active Directory (AD) rakenduste loomisel kõige levinumate probleemide tõrkeotsinguks lugege järgmisi artikleid.

- [Näen probleeme ainult Chrome ' i brauseri kaudu sisselogimisel rakendusse (desse)](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Ma ei tea, kuidas muuta rakenduse turbelubade kasutuse vaikesätteid](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Olen segaduses selle pärast, kuidas rakenduse nõusolek töötab](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Ma ei tea, kuidas oma rakendusele lube anda](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Ma ei saa aru delegeeritud ja rakenduse kasutusõiguste erinevusest](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Azure Active Directory autentimise teegi (ADAL) ja AZURE ad Graph API (AAD Graph) _ toe lõppemine**

- Alates 30 juunist 2020 ei lisa me enam Azure Active Directory autentimise teeki (ADAL) ja Azure AD Graph API-d (AAD Graph) uusi funktsioone. Jätkame tehnilise toe ja turvavärskenduste esitamist, kuid ei paku enam funktsioonide värskendusi.

- Alates 30 juunist 2022, lõpetame ADAL ja AAD graafiku toe ning ei paku enam tehnilist tuge ega turvavärskendusi. Selle tingimuse tulemusena on järgmised tagajärjed.

    - Rakendused, mis kasutavad ADAL olemasolevatel OPERATSIOONISÜSTEEMI versioonidel, jätkavad tööd ka pärast seda, kuid ei saa tehnilist tuge ega turvavärskendusi.

    - Rakendused, mis kasutavad AAD Graph ' i, ei pruugi enam saada vastuseid AAD Graph Endpoint

_ *ADAL migreerimine**

Kui kasutate Microsofti rakendusi, soovitame värskendada Microsoft Authenticationi teeki (MSAL), kus on uusimad funktsioonid ja turvavärskendused. See soovitus on Microsofti kontekstis, mille käigus alustatakse selle rakenduste migreerimist MSAL lõpptähtpäeva järgi. 

Microsoft oma rakenduste migreerimine MSAL tagab, et rakendused saavad kasu MSAL pidevast turbest ja funktsioonide täiustustest.

1. [Lugege ADAL KKK-sid](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Vaadake, kuidas rakendusi ühe platvormi põhjal migreerida](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Kui vajate abi selle mõistmisel, mida teie rakendused kasutavad ADAL, soovitame teil kõigi rakenduste lähtekoodi üle vaadata ja vajaduse korral jõuda kõigi sõltumatute tarkvara tarnijate (tarkvaratoode) või rakenduste pakkujatega. Microsofti tugiteenused võivad anda teile ka kõigi teie rentniku jaoks mitte-Microsofti ADAL rakenduste loendi.

**AAD Graphi migreerimine**

Kui teil on rakenduses AAD Graph kasutatavaid rakendusi, järgige meie juhiseid AAD Graph ' i rakenduste migreerimiseks Microsoft Graphi.

1. [Meie migreerimise kontroll-loend on](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)alustamine. 
2. Teie Azure ' i rakenduse registreerimise portaal näitab, millised rakendused kasutavad AAD graafikut. Soovitame üle vaadata kõik rakenduste lähtekoodi ja vajaduse korral jõuda iseseisvate tarkvara tarnijate (tarkvaratoode) või rakenduste pakkujatega. Microsofti tugiteenused võivad anda teile teavet ka teie rentniku AAD Graphi kasutamise kohta.







