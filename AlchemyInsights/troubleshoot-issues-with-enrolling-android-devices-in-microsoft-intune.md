---
title: Tõrkeotsingu kasutamine Microsoft Intune Android seadmete
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 6b26b2d77bceb063090986ff4e20bc4a56bb1242
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29655879"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Tõrkeotsingu kasutamine Microsoft Intune Android seadmete

Läbi nende lahendamiseks nüüd allpool loetletud ressurssidele.
  
Mõned levinud probleemid ja lahendus:
  
 **Seadme krüptimata Ettevõtjaportaal viga:** Android, eriti alates v7.0, uuemad versioonid nõuavad pääsukoodi käivitamisel veenduge, et seade on täielikult krüptitud. Käivituse PIN-koodi või täielikult seadme krüptimine on ühiseid lahendusi. Läbi [selle dokumendi](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) lisateabe. 
  
 **Seadmed ei saate Intune service sisse või kuvada Intune konsoolis "Unhealthy":** Mõned Samsung 4.4 ja 5,5 seadmed võivad kontrolli teenindusse. Seal on 3 võimalikud lahendused selle probleemi: 
  
1. Käsitsi avada Intune Ettevõtjaportaal app, mis algatab automaatselt seadme sünkroonimine.
    
2. Värskendage seadme Android 6.0 või kõrgem.
    
3. Keelata Samsung Smart Manager hallata Intune'i Ettevõtjaportaal. Läbi [selle dokumendi](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) täpsemat teavet need probleemid ja lahendused. 
    
 **Kasutaja litsentsi tüüp ei sobi** või **kasutaja nimi tundmatu tõrge:** kasutaja peab olema määratud Intune või EMS litsentsi. Läbi nende dokumentide kaudu litsentsi omistamiseks: Office administreerimiskeskuse või Azure portaali. 
  
Lisaressursse, mis probleemi lahendada:
  
1. Diagnoosimiseks ja lahendamiseks ühise registreerimise rikete [Intune tõrkeotsingu portaali](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) abil. Läbi [selle dokumendi](https://docs.microsoft.com/intune/help-desk-operators) lisateabe saamiseks. 
    
2. Nimekiri kõige sagedasemad vead, mis takistavad registreerimine ja lahendused igale [dokumendi](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) läbivaatamiseks. 
    
3. [Kuidas registreeruda Microsoft Intune Androidiga](https://docs.microsoft.com/intune/android-enroll).
    

