---
title: Tõrkeotsingu kasutamine iOS seadmeid Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: d28dca4fccf823e627dd179f828ba3b8baf843a6
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29924764"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Tõrkeotsingu kasutamine iOS seadmeid Microsoft Intune

Läbi nende lahendamiseks nüüd allpool loetletud ressurssidele. 
  
Mõned levinud tõrketeated ja lahendus:
  
- **Seadme Cap jõudis** Kasutajal on rohkem kui seadme seadmete. Läbi nende dokumentide [seade eemaldada](https://docs.microsoft.com/intune/devices-wipe) või [muuta seadme piirang](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **See teenus ei toeta. Puudub liitumise poliitika:** Apple Push teatamise teenus (APNid) määramine peab olema konfigureeritud või uuendada. Läbi [selle dokumendi](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) juhiseid, kuidas seda teha. 
    
- **Kasutaja litsentsi tüüp sobimatu või Tundmatu kasutajanimi:** Kasutaja peab olema määratud Intune või EMS litsentsi. Läbi nende dokumentide kaudu litsentsi omistamiseks: [Office administreerimiskeskuse](https://docs.microsoft.com/intune/licenses-assign) või [Azure'i portaal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Lisaressursse, mis probleemi lahendada:
  
1. Diagnoosimiseks ja lahendamiseks ühise registreerimise rikete [Intune tõrkeotsingu portaali](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) abil. Läbi [selle dokumendi](https://docs.microsoft.com/intune/help-desk-operators) lisateabe saamiseks. 
    
2. Läbi nende dokumentide nimekiri kõige sagedasemad vead, mis takistavad registreerimine ja lahendused igale: [tõrkeotsing juhend](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ja [tõrkeotsing doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Kuidas registreeruda Microsoft Intune iOS seadmeid](https://docs.microsoft.com/intune/ios-enroll).
    

