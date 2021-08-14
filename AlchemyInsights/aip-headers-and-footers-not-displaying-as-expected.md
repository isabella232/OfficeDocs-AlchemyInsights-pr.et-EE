---
title: 'AIP: päised ja jalused ei kuvata ootuspäraselt'
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
- "9002266"
- "4541"
ms.openlocfilehash: e3a0e5caccba87ddd8e4c786b5c8918494e709b6f4d5d60e7c31215a60b1d5d6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951777"
---
# <a name="aip-headers-and-footers-not-displaying-as-expected"></a>AIP: päised ja jalused ei kuvata ootuspäraselt

Kui teil on probleeme nägemismärkidega, mida ei kuvata ootuspäraselt, vaadake järgmisi juhiseid.

1. Veenduge, et olete [visuaalsete märgistuste rakendades läbi vaadanud.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. Siltide Office vaadake läbi, [kui Office 365 rakendab sisumärgistuse ja krüptimise.](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps#when-office-apps-apply-content-marking-and-encryption)
3. Kui soovite olemasolevad päised/jalused eemaldada, vaadake läbi [Päiste ja jaluste eemaldamine muudest sildistamislahendustest.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-customizations#remove-headers-and-footers-from-other-labeling-solutions)

Kui probleem ei kao, koguge Azure'i teabekaitse kliendi logid ja manustage eksporditud logid sellele piletile.

**Azure'i teabekaitse logide eksportimine**

1. Avage Office või looge uus meilisõnum Outlook.
2. Klõpsake **nuppu Kaitse/tundlikkuse**  >  **spikker ja tagasiside.**
3. Klõpsake **nuppu Ekspordi logid.**
4. Salvestage logid oma asukohavalikusse ja manustage need sellele teenusetaotlusele.

Lisateavet leiate teemast

- [Azure'i teabekaitse jaoks visuaalsete märgistuste sildi konfigureerimine](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Azure'i teabekaitse dokumentatsiooni läbivaatamine](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Azure'i teabekaitse nõuded](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Azure'i teabekaitse lühikäivitusõpetus](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Azure'i teabekaitse kliendi allalaadimine](https://www.microsoft.com/download/details.aspx?id=53018)
