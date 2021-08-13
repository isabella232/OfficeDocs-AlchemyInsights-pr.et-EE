---
title: Windows seadmete Microsoft Intune
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
ms.openlocfilehash: a2abb4d0ef5504c496afefe62a80f3fa21c7ec85536e822e402be33b3617b59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981037"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Windows seadmete Microsoft Intune

Vaadake allpool loetletud ressursid üle, et probleem kohe lahendada.
  
Levinumad tõrketeated ja eraldusvõime juhised.
  
 **Tarkvara ei saa installida, 0x80cf4017.** Teie konto sert on aegunud. Laadige PC-kliendi tarkvarapakett Intune'i halduskonsoolis uuesti alla. Lisateabe saamiseks vaadake seda dokumentatsiooni.
  
 **Tõrkekood 0x801c0003:** Tõrge võib ilmneda järgmistel juhtudel.
  
-  Kasutajal on rohkem seadmeid, mis on registreeritud kui seadme limiit. Vaadake need dokumendid [üle, et eemaldada seade](https://docs.microsoft.com/intune/devices-wipe) [või muuta seadme piirangut.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  "Kasutajad võivad seadmetega Azure AD-ga liituda" on seatud väärtusele "pole". Määrake see kõigile või valige kasutajad. Lisateabe [saamiseks vaadake](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) seda dokumentatsiooni.

-  Teine kasutaja on seadme juba registreerinud. Sel juhul eemaldage seade Azure Intune'i konsoolist või eemaldage seade enne uuesti proovimist käsitsi.

-  Seade on Windows 10 Home. Ainult Windows 10 Pro, haridusasutuste ja ettevõtete SSK-d saavad Azure Active Directory.

Täiendavad ressursid probleemi lahendamiseks.
  
-  [Intune'i tõrkeotsinguportaali](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) abil saate diagnoosida ja lahendada levinumaid registreerimistõrkeid. Lisateavet [leiate sellest](https://docs.microsoft.com/intune/help-desk-operators) dokumendist.

-  Vaadake need dokumendid üle, et saada ülevaade levinumatest vigadest, mis takistavad registreerimist ja lahendamist: tõrkeotsingu [juhend ja](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) [tõrkeotsingu dokument.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

[Saate teada, kuidas Windows seadmetesse Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)
