---
title: Üleminek AIP-ist kuni MIP/ühtse märgistamiseni vastavuse keskuses
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
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674322"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Üleminek AIP-ist kuni MIP/ühtse märgistamiseni vastavuse keskuses

Üleminekuks AIP-i siltidelt turbe-ja vastavuskontrolli keskuses ühendatud siltidele tehke järgmist.

**Azure ' i portaalis kaitse aktiveerimine**

1. Kui te pole seda veel teinud, avage uus brauseriaknas ja [logige sisse Azure ' i portaali](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Liikuge **Azure ' i teabe kaitse** labale. Näiteks klõpsake menüüs keskus käsku **kõik teenused** ja hakake tippima **teavet** väljale filter. Valige **Azure ' i teabe kaitse**. Kui te pole Azure ' i teabe kaitse Blade ' i varem kasutanud, lugege [lisajuhiseid](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) selle tera lisamiseks portaali. Azure ' i teabe kaitse Blade avamiseks peab teil olema kas Azure ' i [teabe kaitse Premiumi leping](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) või Office 365 leping, mis sisaldab õiguste haldust. Kui teil on üks neist tellimustest, kuid kuvatakse teade selle kohta, et kehtivat tellimust ei leita, [võtke ühendust Microsofti toega](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) või kasutage standardseid kasutajatoe kanaleid.

2. Leidke menüü **Halda** suvandid ja valige **kaitse aktiveerimine**. Klõpsake nuppu **Aktiveeri**ja seejärel kinnitage oma toiming. Kui aktiveerimine on lõpule jõudnud, kuvab teaberiba **aktiveerimine edukalt**.

**Azure ' i teabe kaitse siltide migreerimine Office 365 turbe & nõuetele vastavuse keskuses**

1. Veenduge, et olete sisse logitud üldise administraatori õigustega kasutajana.

2. Liikuge **Azure ' i teabe kaitse** labale.

3. Valige menüüst **Halda** suvand **ühendatud silt**.

4. Klõpsake **Azure ' i teabe kaitsega ühendatud sildiga** Blade nuppu **Aktiveeri** ja järgige veebijuhiseid.

**Märkus**: Veenduge, et teil oleks enne turbe & ühilduvuse keskuse migreerimise aktiveerimiseks vajalikud load. Lisateavet leiate järgmistest artiklitest:

1. [Kas peate Azure ' i teabe kaitse konfigureerimiseks olema üldadministraator või saan anda teistele administraatoritele delegaadi?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Oluline teave administratiivsete rollide kohta pärast turbe & nõuetele vastavuse keskuse migreerimist.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Lisateavet AIP-i kohta, et ühendatud siltide migreerimine turbe-ja vastavuskontrolli keskusse, leiate teemast [siltide migreerimine](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
