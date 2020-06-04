---
title: Microsofti Intune ' i Windowsi seadmetega seotud probleemide tõrkeotsing
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665828"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Microsofti Intune ' i Windowsi seadmetega seotud probleemide tõrkeotsing

Vaadake allpool loetletud ressursid probleemi lahendamiseks kohe.
  
Mõned levinud tõrketeated ja eraldusvõime sammud:
  
 **Tarkvara ei saa installida, 0x80cf4017:** Teie kontosert on aegunud. Uuesti alla laadida arvuti kliendi tarkvarapakett Intune konsoolis. Lisateabe saamiseks vaadake seda dokumentatsiooni.
  
 **Tõrkekood 0x801c0003:** Tõrge võib ilmneda järgmistel juhtudel:
  
-  Kasutajal on rohkem seadmeid, mis on registreeritud kui seadme piirang. Vaadake neid dokumente [seadme eemaldamiseks](https://docs.microsoft.com/intune/devices-wipe) või [seadme piirangu muutmiseks](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Kasutajad võivad liituda seadmete Azure AD" on seatud "none." Seadke see kõigile või valige kasutajad. Lisateabe saamiseks vaadake [seda dokumentatsiooni](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .

-  Seade on juba teise kasutaja poolt registreeritud. Kui see on nii, eemaldage seade Azure Intune konsooli või enne uuesti proovimist seadme käsitsi lahti.

-  Seade on Windows 10 Home. Azure Active Directoryga saab liituda ainult Windows 10 Pro, haridus ja Enterprise SKUs.

Täiendavad ressursid probleemi lahendamiseks:
  
-  Levinud registreerimise tõrgete diagnoosimiseks ja lahendamiseks kasutage [tõrkeotsingu portaali Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) . Vaadake [seda dokumenti](https://docs.microsoft.com/intune/help-desk-operators) rohkem üksikasju.

-  Vaadake need dokumendid läbi levinud tõrgete loendi, mis takistavad registreerimise ja resolutsioonide iga: [tõrkeotsingu juhend](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ja [tõrkeotsingu doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Vaadake, kuidas Windowsi seadmeid Microsoft Intune ' is registreeruda](https://docs.microsoft.com/intune/windows-enroll).
