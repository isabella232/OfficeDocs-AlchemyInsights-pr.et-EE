---
title: Microsoft Intune'is Windowsi seadmete registreerimisega seotud probleemide tõrkeotsing
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808967"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Microsoft Intune'is Windowsi seadmete registreerimisega seotud probleemide tõrkeotsing

Vaadake allpool loetletud ressursid üle, et probleem kohe lahendada.
  
Levinumad tõrketeated ja eraldusvõime juhised.
  
 **Tarkvara ei saa installida, 0x80cf4017.** Teie konto sert on aegunud. Laadige PC-kliendi tarkvarapakett Intune'i halduskonsoolis uuesti alla. Lisateabe saamiseks vaadake seda dokumentatsiooni.
  
 **Tõrkekood 0x801c0003:** Tõrge võib ilmneda järgmistel juhtudel.
  
-  Kasutajal on rohkem seadmeid, mis on registreeritud kui seadme limiit. Vaadake need dokumendid [üle, et eemaldada seade](https://docs.microsoft.com/intune/devices-wipe) [või muuta seadme piirangut.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  "Kasutajad võivad seadmetega Azure AD-ga liituda" on seatud väärtusele "pole". Määrake see kõigile või valige kasutajad. Lisateabe [saamiseks vaadake](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) seda dokumentatsiooni.

-  Teine kasutaja on seadme juba registreerinud. Sel juhul eemaldage seade Azure Intune'i konsoolist või eemaldage seade enne uuesti proovimist käsitsi.

-  Seade on Windows 10 Home. Azure Active Directoryga saavad liituda ainult Windows 10 Pro, Education ja Enterprise SKUs.

Täiendavad ressursid probleemi lahendamiseks.
  
-  [Intune'i tõrkeotsinguportaali](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) abil saate diagnoosida ja lahendada levinumaid registreerimistõrkeid. Lisateavet [leiate sellest](https://docs.microsoft.com/intune/help-desk-operators) dokumendist.

-  Vaadake need dokumendid üle, et saada ülevaade levinumatest vigadest, mis takistavad registreerimist ja lahendamist: tõrkeotsingu [juhend ja](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) [tõrkeotsingu dokument.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

[Saate teada, kuidas registreerida Windowsi seadmeid Microsoft Intune'is.](https://docs.microsoft.com/intune/windows-enroll)
