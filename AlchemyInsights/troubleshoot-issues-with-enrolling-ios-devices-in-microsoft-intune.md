---
title: Microsoft Intune ' i sisseveeretavate iOS-i seadmetega seotud probleemide tõrkeotsing
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36506921"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Microsoft Intune ' i sisseveeretavate iOS-i seadmetega seotud probleemide tõrkeotsing

Vaadake allpool loetletud ressursid probleemi lahendamiseks kohe. 
  
Mõned levinud tõrketeated ja eraldusvõime sammud:
  
- **Seadme kork on saavutatud** Kasutajal on rohkem seadmeid, mis on registreeritud kui seadme piirang. Vaadake neid dokumente [seadme eemaldamiseks](https://docs.microsoft.com/intune/devices-wipe) või [seadme piirangu muutmiseks](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Seda teenust ei toetata. Ei ole registreerimine poliitika:** Apple push Notification Service (APNS) tuleb konfigureerida või uuendada. Vaadake [seda dokumenti](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) juhiste saamiseks selle kohta, kuidas seda teha. 
    
- **Kasutaja litsentsi tüüp kehtetu või kasutaja nimi ei tuvastata:** Kasutajale tuleb määrata Intune ' i või EMS-i litsents. Vaadake üle need dokumendid litsentsi määramiseks: [Office ' i halduskeskus](https://docs.microsoft.com/intune/licenses-assign) või [Azure ' i portaal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Täiendavad ressursid probleemi lahendamiseks:
  
1. Levinud registreerimise tõrgete diagnoosimiseks ja lahendamiseks kasutage [tõrkeotsingu portaali Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) . Vaadake [seda dokumenti](https://docs.microsoft.com/intune/help-desk-operators) rohkem üksikasju. 
    
2. Vaadake need dokumendid läbi levinud tõrgete loendi, mis takistavad registreerimise ja resolutsioonide iga: [tõrkeotsingu juhend](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ja [tõrkeotsingu doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Teave selle kohta, kuidas registreeruda iOS-i seadmeid Microsoft Intune ' is](https://docs.microsoft.com/intune/ios-enroll).
    

