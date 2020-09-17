---
title: Juurdepääs Intune ' i tingimustega
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807655"
---
# <a name="conditional-access-with-intune"></a>Juurdepääs Intune ' i tingimustega

Intune  **' i**  kasutamine Intune ' i abil nõuab kolme toimingut.

- Saate luua  **nõuetele vastavuse poliitika**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), et määratleda sätted, mis peavad olema täidetud enne, kui seade on nõuetele vastavaks loetud. Näiteks peab seadmel olema vähemalt 6-kohaline PIN-kood, enne kui seda loetakse nõuetele vastavaks.
- Saate luua **tingimusjuurdepääsu poliitika**  , mis määratleb, milliseid ressursse kaitstakse, ja milliseid tingimusi tuleb nendele ressurssidele juurdepääsuks täita.  [Näiteks](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  peab seade olema ühilduv enne ettevõtte e-postile juurdepääsu.
- Veenduge, et nii **nõuetele vastavuse poliitikad**  kui ka  **tingimusjuurdepääsu poliitikad**  on suunatud soovitud kasutajate rühmadele. See võib nõuda Azure Active Directorys teatud kasutajate rühmade loomist.

**Kasulikud lingid:**

[Seadme nõuetele vastavuse ülevaade](https://docs.microsoft.com/intune/device-compliance-get-started)

[Tõrkeotsing CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Tõrkeotsingu poliitika](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Meili (Exchange Online) ' i kaitsmiseks lubamatute seadmete kaudu juurdepääsu eest tuleb järgida mõlemat dokumenti.

1. [E-posti kaitse kasutamine EAS-i kasutavates seadmetes](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Meilikontode kaitsmine seadmete kaudu, mis kasutavad kaasaegseid autentimise kliente (nt Outlook)](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)