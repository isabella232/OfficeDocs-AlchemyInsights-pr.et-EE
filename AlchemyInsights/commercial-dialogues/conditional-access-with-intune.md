---
title: Tingimusjuurdepääsu kasutamine Intune'iga
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 23afea21668191093d612d68ca6e9ab2a844f4a14977631d33f4fd956fc3c4e7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005770"
---
# <a name="using-conditional-access-with-intune"></a>Tingimusjuurdepääsu kasutamine Intune'iga

Tingimusjuurdepääsu kasutamine Intune'iga nõuab 3 etappi.

- [Looge vastavuspoliitika, et määratleda sätted, mis peavad olema täidetud enne, kui seade loetakse nõuetele vastavaks. Näiteks peab seadmel olema vähemalt 6-kohaline pin-kood, enne kui seda peetakse nõuetele vastavaks.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Looge tingimusjuurdepääsu poliitika, mis määratleb, millised ressursid on kaitstud ja millistele tingimustele tuleb nendele ressurssidele juurdepääsemiseks täita. Näiteks peab seade enne ettevõtte meilide kasutamist vastama nõuetele.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Veenduge, et nii vastavuspoliitikad kui ka tingimusjuurdepääsu poliitikad on suunatud soovitud kasutajarühmadele. See võib nõuda teatud kasutajarühmade loomist Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Lugege lisateavet...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
