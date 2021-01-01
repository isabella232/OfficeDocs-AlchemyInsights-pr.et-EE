---
title: Azure’i arvelduse omanduse ülekandmine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: 454ce626862bb4a2361abccd92ad0099b534388c
ms.sourcegitcommit: 059ad2936788266ea9714ec8c66d407d7261aeb6
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 12/29/2020
ms.locfileid: "49736874"
---
# <a name="transfer-azure-billing-ownership"></a>Azure’i arvelduse omanduse ülekandmine

Logige [Azure’i portaali](https://portal.azure.com/) sisse selle arvelduskonto administraatorina, millel on tellimus, mida soovite üle kanda. Kui te pole kindel, kas olete administraator, või peate kindlaks tegema, kes on, avage valik [Konto arveldusadministraatori kindlakstegemine](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

1. Otsige üksusest _Kuluhaldus ja arveldus_.
1. Valige vasakpoolselt paanilt **Tellimused**. Olenevalt juurdepääsust on võimalik, et peate valima arveldusulatuse ja seejärel valiku **Tellimused** või **Azure’i tellimused**.
1. Valige selle tellimuse puhul, mida soovite üle kanda, käsk **Kanna üle arvelduse omandus**.
1. Sisestage selle kasutaja meiliaadress, kes on selle konto arveldusadministraator, millest saab tellimuse uus omanik, ja seejärel valige käsk **Saada ülekandmistaotlus**.
1. Kasutajale saadetakse meil koos juhtnööridega teie ülekandmistaotluse läbivaatamiseks. Ülekandmistaotluse kinnitamiseks peab kasutaja valima meilis toodud lingi ja järgima juhtnööre.

Kui kannate tellimuse arvelduse omanduse üle kasutaja kontole, mis asub teises Azure AD rentnikus, eemaldatakse jäädavalt kõik [rollipõhise juurdepääsu reguleerimise](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) määramised tellimuse ressursside haldamiseks. Ainult uuel omanikul on juurdepääs tellimuse ressursside haldamiseks. Lisateavet selle kohta, kuidas muuta tellimuse kataloogi, leiate teemast [Tellimuse ülekandmine teises Azure AD rentnikus asuvale kasutajale](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

_**Oluline mõju teie arvetele**_: kui olete Azure’i tellimuse omanduse üle kandnud, on teie tasud proportsionaalsed. Arvetele pääsete juurde järgmiselt.  

1. Valige [Azure’i portaali](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) tellimuste lehelt [kasutajana, kellel on juurdepääs arvetele, oma tellimus](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)ja seejärel valige **Arved**.
1. PDF-arve koopia vaatamiseks klõpsake käsku  **Laadi arve alla** . Kui kuvatakse teade _Pole saadaval_, avage [Miks ma ei näe viimase arveldusperioodi arvet?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice).
1. Päevakasutust saate vaadata, kui klõpsate **arveldusperioodi**. Nii saate oma arve PDF-i ja üksikasjaliku päevakasutuse faili (.CSV) koopia. Lisateavet leiate teemast  [Arve ja kasutusandmete hankimine](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support).

**Soovitatud dokumendid**

- [Azure’i tellimuse arvelduse omanduse ülekandmine teisele kontole](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Teave Azure’i tellimuse arvelduse omanduse ülekandmise kohta](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Visual Studio, Microsoft Partner Networki ja Pay as you go arendus-/testtellimuste ülekandmine](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Omanduse ülekandmise KKK](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Omanduse ülekandmise probleemide tõrkeotsing](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
