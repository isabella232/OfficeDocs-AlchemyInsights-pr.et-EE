---
title: Tingimusjuurdepääs Intune'iga
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c24451fba8b8ab8fe7a1778bb292dec6678e1ef487076d27458c9aeb4963c683
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069708"
---
# <a name="conditional-access-with-intune"></a>Tingimusjuurdepääs Intune'iga

**Tingimusjuurdepääsu** kasutamine Intune'iga nõuab 3 etappi.

- Looge **vastavuspoliitika** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) sätete määratlemiseks, mis peavad olema täidetud enne, kui seade loetakse nõuetele vastavaks. Näiteks peab seadmel olema vähemalt 6-kohaline pin-kood, enne kui seda peetakse nõuetele vastavaks.
- Looge **tingimusjuurdepääsu poliitika,**  mis määratleb, millised ressursid on kaitstud ja millistele tingimustele tuleb nendele ressurssidele juurdepääsemiseks täita.  [Näiteks peab seade](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  enne ettevõtte meilide kasutamist vastama nõuetele.
- Veenduge, et nii **vastavuspoliitikad** kui ka tingimusjuurdepääsu poliitikad on suunatud soovitud kasutajarühmadele.  See võib nõuda teatud kasutajarühmade loomist Azure Active Directory.

**Kasulikud lingid:**

[Seadme nõuetele vastavuse ülevaade](https://docs.microsoft.com/intune/device-compliance-get-started)

[Ca tõrkeotsing](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Tõrkeotsingupoliitika](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Meiliteenuse (Exchange veebiversioon) kaitsmiseks mittepädevate seadmete juurdepääsu eest tuleb järgida mõlemat dokumenti.

1. [Meilijuurdepääsu kaitsmine seadmetes EAS-i abil](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Meilijuurdepääsu kaitsmine seadmetes, kus kasutatakse modernautentimise kliente (Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)