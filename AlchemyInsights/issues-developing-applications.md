---
title: Rakenduste arendamisega seotud probleemid
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
ms.openlocfilehash: 065ff6d965063e44c4d1771821985058c9d020fbbabb0d381f30b6a11132c4ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013420"
---
# <a name="issues-developing-applications"></a>Rakenduste arendamisega seotud probleemid

Levinumate probleemide tõrkeotsinguks Azure Active Directory (AD) rakenduste loomiseks lugege järgmisi artikleid.

- [Mul on probleeme ainult Chrome'i brauseri abil rakendusse (rakendustesse) sisselogimisega](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Ma ei tea, kuidas muuta rakenduse lubade kasutusaja vaikesätet](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Olen segaduses selle pärast, kuidas rakenduse nõusolek toimib](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Ma ei tea, kuidas anda oma rakendusele õigusi](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Ma ei mõista delegeeritud õiguste ja rakenduseõiguste erinevust](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Autentimisteegi (ADAL) Azure Active Directory Azure AD Graph API (AAD Graph) tugi***

- Alates 30. juunist 2020 ei lisa me enam uusi funktsioone Azure Active Directory autentimisteeki (ADAL) ja Azure AD Graphi API-sse (AAD Graphi). Pakume endiselt tehnilist tuge ja turbevärskendusi, ent mitte enam funktsioonivärskendusi.

- Alates 30. juunist 2022 lõpetame ADAL-i ja AAD Graphi tootetoe ega paku enam tehnilist tuge ega turbevärskendusi. Selle tingimuse tõttu on järgmised tagajärjed.

    - Olemasolevates opsüsteemiversioonides ADAL-i kasutavad rakendused töötavad edasi ka pärast seda, ent ei saa enam tehnilist tuge ega turbevärskendusi.

    - Rakendused, mis kasutavad AAD Graph i pärast seda aega, ei pruugi enam AAD-Graph vastuseid

**ADAL-migreerimine**

Kui kasutate Microsofti rakendusi, soovitame üle võtta Microsofti autentimisteegi (MSAL), mis sisaldab uusimaid funktsioone ja turbevärskendusi. See soovitus on Seotud Microsoftiga, kes algatab oma rakenduste MSAL-i migreerimise toe lõpu tähtajaks. 

Microsofti rakenduste migreerimine MSAL-i tagab, et rakendused saavad msal-i turbe- ja funktsioonitäiustustest kasu.

1. [Lugege ADAL-i KKK-d.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Lugege lisateavet rakenduste platvormipõhise migreerimise kohta.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Kui vajate abi selle mõistmisel, milline teie rakendus ADAL-i kasutab, soovitame teil läbi vaadata kõik rakenduste lähtekoodid ja vajaduse korral ühendust võtta mis tahes sõltumatu tarkvara tarnija (ISV) või rakendusepakkujaga. Samuti saab Microsofti tugi anda teile nimekirja kõigist neist mitte-Microsofti rakendustest teie rentnikkeskkonnas, mis kasutavad ADAL-i.

**AAD Graphi migreerimine**

Rakenduste puhul, mis kasutavad AAD-Graph, järgige meie juhiseid AAD-Graph migreerimiseks Microsofti Graph.

1. [Meie migreerimise kontroll-loend on hea koht alustamiseks](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Azure‘i rakenduste registreerimisportaalis näete, millised rakendused kasutavad AAD Graphi. Soovitame läbi vaadata kõik rakenduste lähtekoodid ja vajaduse korral ühendust võtta mis tahes sõltumatu tarkvara tarnija (ISV) või rakendusepakkujaga. Microsofti tugiteenuste abil saate teavet ka rentniku Graph kasutamise kohta.







