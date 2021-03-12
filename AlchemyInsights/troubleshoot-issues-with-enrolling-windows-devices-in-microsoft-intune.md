---
title: Windowsi seadmete registreerimisega seotud probleemide tõrkeotsing Microsoft Intune ' is
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708886"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Windowsi seadmete registreerimisega seotud probleemide tõrkeotsing Microsoft Intune ' is

Probleemi lahendamiseks vaadake allpool loetletud ressursid üle.
  
Levinumad tõrketeated ja eraldusvõime toimingud.
  
 **Tarkvara ei saa installida, 0x80cf4017.** Teie konto sert on aegunud. Laadige PC-kliendi tarkvarapakett uuesti alla Intune konsoolis. Lisateabe saamiseks vaadake seda dokumentatsiooni.
  
 **Tõrkekood 0x801c0003:** Tõrge võib ilmneda järgmistel juhtudel.
  
-  Kasutajal on rohkem seadmeid, kui seadme limiit on registreeritud. Vaadake need dokumendid üle, et [seade eemaldada](https://docs.microsoft.com/intune/devices-wipe) või [muuta seadme limiiti](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Kasutajad võivad ühendada seadmed Azure AD" on seatud "pole". Määrake see kõigile või valige kasutajad. Lisateabe saamiseks vaadake [seda dokumentatsiooni](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .

-  Teine kasutaja on seadme juba registreerinud. Kui see on nii, eemaldage seade Azure ' i Intune ' i konsoolist või registreerige seade enne uuesti proovimist käsitsi.

-  Seade on Windows 10 Home. Azure Active Directoryga saab liituda ainult Windows 10 Pro, haridusasutuste ja Enterprise ' i SKUs.

Probleemi lahendamiseks täiendavad ressursid.
  
-  Saate kasutada [Intune tõrkeotsingu portaali](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) levinud liitumise tõrgete diagnoosimiseks ja lahendamiseks. Lisateabe saamiseks vaadake [seda dokumenti](https://docs.microsoft.com/intune/help-desk-operators) üle.

-  Vaadake need dokumendid läbi nende levinud tõrgete loend, mis takistavad iga kasutaja registreerimist ja eraldusvõimet: [veaotsingu tõrkeotsing](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ja [tõrkeotsingu dokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).

[Siit saate teada, kuidas Windowsi seadmeid Microsoft Intune ' is registreerida](https://docs.microsoft.com/intune/windows-enroll).
