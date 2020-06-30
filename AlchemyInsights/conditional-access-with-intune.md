---
title: Tingimuslik juurdepääs Intune'iga
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931426"
---
# <a name="conditional-access-with-intune"></a>Tingimuslik juurdepääs Intune'iga

**Tingimusjuurdepääsu** kasutamine Intune'iga nõuab kolme etappi.

- Looge **vastavuspoliitika** [(Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), et määratleda sätted, mis peavad olema täidetud enne seadme nõuetele vastavust. Näiteks peab seadmel olema vähemalt 6-kohaline viik, enne kui seda loetakse nõuetele vastavaks.
- Looge **tingimusjuurdepääsu poliitika,** mis määratleb, milliseid ressursse kaitstakse ja millised tingimused peavad nendele ressurssidele juurdepääsuks olema täidetud.  [Näiteks](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) seade peab olema ühilduv enne juurdepääsu ettevõtte e-posti.
- Veenduge, et nii **vastavuspoliitika** kui ka **tingimusjuurdepääsu poliitika** on suunatud soovitud kasutajarühmadele. See võib nõuda teatud kasutajate rühmade loomine Azure Active Directorys.

**Kasulikud lingid:**

[Seadme vastavuse ülevaade](https://docs.microsoft.com/intune/device-compliance-get-started)

[Ca tõrkeotsing](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Tõrkeotsingu poliitika](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Meili (Exchange Online'i) kaitsmiseks mitteühilduvate seadmete juurdepääsu eest tuleb järgida mõlemat dokumenti.

1. [EAS-i abil e-posti juurdepääsu kaitsmine seadmete eest](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Kaitske e-posti juurdepääsu seadmetest, mis kasutavad kaasaegseid autentimiskliente nagu Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)