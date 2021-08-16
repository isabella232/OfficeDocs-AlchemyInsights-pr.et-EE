---
title: Migreerimine AIP-st MIP-sse/ühtseks sildistuskeskuses
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 378c3f58f77db8b23682432c942cd4f9c3a392651ca6564528a635724ad66a25
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000352"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Migreerimine AIP-st MIP-sse/ühtseks sildistuskeskuses

Turbe- ja vastavuskeskuses AIP-siltidelt ühtsele sildistusele migreerimiseks tehke järgmist.

**Kaitse aktiveerimine Azure'i portaali kaudu**

1. Kui te pole seda veel teinud, avage uus brauseriaken ja [logige sisse Azure'i portaali.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal) Liikuge **Azure'i teabekaitse terale.** Näiteks klõpsake jaoturi menüüs käsku **Kõik teenused** ja hakake **tippima väljale** Filter teksti Teave. Valige **Azure'i teabekaitse**. Kui te pole varem Azure'i teabekaitse labale [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) juurde pääsenud, lugege selle lõiketera portaali lisamiseks järgmisi täiendavaid juhiseid. Azure'i teabekaitse tera avamiseks peab teil olema [Kas Azure'i teabekaitse Premium või](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) Office 365, mis sisaldab õiguste haldust. Kui teil on mõni neist tellimustest, kuid kuvatakse teade, et kehtivat tellimust ei leita, pöörduge [Microsofti toe poole](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) või kasutage oma standardseid tugikanaleid.

2. Otsige üles **menüü haldamissuvandid** ja valige **Kaitse aktiveerimine.** Klõpsake **nuppu** Aktiveeri ja seejärel kinnitage oma toiming. Kui aktiveerimine on lõpule viidud, kuvatakse teaberibal teade **Aktiveerimine on edukalt lõpule viidud.**

**Azure'i teabekaitse siltide migreerimine Office 365 turbe- & vastavuskeskusesse**

1. Veenduge, et olete sisse logitud üldadministraatori õigustega kasutajana.

2. Liikuge **Azure'i teabekaitse terale.**

3. Valige **menüüs Halda** käsk **Ühendatud sildistamine**.

4. Klõpsake **Azure'i teabekaitse – ühtse sildistussaba** nuppu **Aktiveeri** ja täitke veebijuhised.

**Märkus.** Enne turbe- ja vastavuskeskuse migreerimise aktiveerimist veenduge, et teil & õigused. Lisateavet leiate nendest artiklitest.

1. [Kas teil peab olema Azure'i teabekaitse konfigureerimiseks üldadministraator või saan delegeerida selle teistele administraatoritele?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Oluline teave haldusrollide kohta pärast turbe- ja vastavuskeskusesse & migreerimist.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Lisateavet AIP ühtse sildistuse migreerimise kohta turbe- ja vastavuskeskusesse leiate teemast [Siltide migreerimine.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)
