---
title: Microsoft Intune'is iOS-i seadmete registreerimisega seotud probleemide tõrkeotsing
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823459"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Microsoft Intune'is iOS-i seadmete registreerimisega seotud probleemide tõrkeotsing

Vaadake allpool loetletud ressursid üle, et probleem kohe lahendada. 
  
Levinumad tõrketeated ja eraldusvõime juhised.
  
- **Seadme suurtähelukk on saavutatud** Kasutajal on rohkem seadmeid, mis on registreeritud kui seadme limiit. Vaadake need dokumendid [üle, et eemaldada seade](https://docs.microsoft.com/intune/devices-wipe) [või muuta seadme piirangut.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Seda teenust ei toetata. Registreerimispoliitika puudub.** Apple'i tõuketeatise teenus (APNS) tuleb konfigureerida või uuendada. Vaadake [läbi see dokument,](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) et saada juhiseid selle kohta, kuidas seda teha. 
    
- **Kasutajalitsentsi tüüp On kehtetu või kasutajanime ei tuvastata.** Kasutajale tuleb määrata Intune'i või EMS-i litsents. Vaadake need dokumendid üle, et määrata litsents [office'i halduskeskuse või](https://docs.microsoft.com/intune/licenses-assign) [Azure'i portaali kaudu.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
Täiendavad ressursid probleemi lahendamiseks.
  
1. [Intune'i tõrkeotsinguportaali](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) abil saate diagnoosida ja lahendada levinumaid registreerimistõrkeid. Lisateavet [leiate sellest](https://docs.microsoft.com/intune/help-desk-operators) dokumendist. 
    
2. Vaadake need dokumendid üle, et saada ülevaade levinumatest vigadest, mis takistavad registreerimist ja lahendamist: tõrkeotsingu [juhend ja](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) [tõrkeotsingu dokument.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)
    
3. [Siit saate teada, kuidas registreerida iOS-i seadmeid Microsoft Intune'is.](https://docs.microsoft.com/intune/ios-enroll)
    

