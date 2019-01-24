---
title: Tõrkeotsingu kasutamine Windowsi seadmetes Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8d19bbd5a5782c7793c87499baf62b2eb7de82ae
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29466541"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Tõrkeotsingu kasutamine Windowsi seadmetes Microsoft Intune

Läbi nende lahendamiseks nüüd allpool loetletud ressurssidele. 
  
Mõned levinud tõrketeated ja lahendus:
  
 **Ei saa installida tarkvara, 0x80cf4017:** Teie konto sert on aegunud. Uuesti laadida PC kliendi tarkvara paketi Intune konsoolis. Läbi selle dokumentatsioonist. 
  
 **Tõrkekood 0x801c0003:** Tõrge võib ilmneda järgmistel juhtudel: 
  
1. Kasutajal on rohkem kui seadme seadmete. Läbi nende dokumentide [seade eemaldada](https://docs.microsoft.com/en-us/intune/devices-wipe) või [muuta seadme piirang](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
2. "Kasutajad võivad ühendada seadmeid Azure AD" on seatud "ei ole". Määrata kõigile või kasutajad. Vaadake lisateabe saamiseks [selle dokumentatsiooni](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) . 
    
3. Mõni teine kasutaja on juba registreeritud seadme. Kui see juhtub, Eemalda seadme Azure Intune konsooli või käsitsi unenroll seade enne uuesti proovimist.
    
4. Seade on Windows 10 Home. Ainult Windows 10 Pro, hariduse ja ettevõtluse SKUs saab liituda Azure Active Directory.
    
Lisaressursse, mis probleemi lahendada:
  
1. Diagnoosimiseks ja lahendamiseks ühise registreerimise rikete [Intune tõrkeotsingu portaali](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) abil. Läbi [selle dokumendi](https://docs.microsoft.com/en-us/intune/help-desk-operators) lisateabe saamiseks. 
    
2. Läbi nende dokumentide nimekiri kõige sagedasemad vead, mis takistavad registreerimine ja lahendused igale: [tõrkeotsing juhend](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ja [tõrkeotsing doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
[Kuidas registreeruda Windowsi seadmetes Microsoft Intune](https://docs.microsoft.com/en-us/intune/windows-enroll).
  

