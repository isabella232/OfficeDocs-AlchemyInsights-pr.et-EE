---
title: IOS-seadmete Microsoft Intune ' is registreerimisega seotud probleemide tõrkeotsing
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708958"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>IOS-seadmete Microsoft Intune ' is registreerimisega seotud probleemide tõrkeotsing

Probleemi lahendamiseks vaadake allpool loetletud ressursid üle. 
  
Levinumad tõrketeated ja eraldusvõime toimingud.
  
- **Seadme kork on täis** Kasutajal on rohkem seadmeid, kui seadme limiit on registreeritud. Vaadake need dokumendid üle, et [seade eemaldada](https://docs.microsoft.com/intune/devices-wipe) või [muuta seadme limiiti](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **See teenus pole toetatud. Pole liitumise poliitikat:** Apple push Notification Service (APNS) peab olema konfigureeritud või uuendatud. Lugege [selle dokumendi](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) juhiseid selle kohta, kuidas seda teha. 
    
- **Kasutaja litsentsi tüüp ei sobi või kasutajanime ei tuvastata:** Kasutajale tuleb määrata Intune või EMS-i litsents. Vaadake need dokumendid üle, et määrata litsents: [Office halduskeskus](https://docs.microsoft.com/intune/licenses-assign) või Azure ' i [portaal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Probleemi lahendamiseks täiendavad ressursid.
  
1. Saate kasutada [Intune tõrkeotsingu portaali](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) levinud liitumise tõrgete diagnoosimiseks ja lahendamiseks. Lisateabe saamiseks vaadake [seda dokumenti](https://docs.microsoft.com/intune/help-desk-operators) üle. 
    
2. Vaadake need dokumendid läbi nende levinud tõrgete loend, mis takistavad iga kasutaja registreerimist ja eraldusvõimet: [veaotsingu tõrkeotsing](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ja [tõrkeotsingu dokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. [Siit saate teada, kuidas Microsoft Intune ' is iOS-i seadmeid registreerida](https://docs.microsoft.com/intune/ios-enroll).
    

