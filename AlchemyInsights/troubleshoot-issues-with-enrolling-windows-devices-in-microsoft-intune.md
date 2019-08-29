---
title: Tõrkeotsingu kasutamine Windowsi seadmetes Microsoft Intune
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
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665828"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Tõrkeotsingu kasutamine Windowsi seadmetes Microsoft Intune

Läbi nende lahendamiseks nüüd allpool loetletud ressurssidele.
  
Mõned levinud tõrketeated ja lahendus:
  
 **Ei saa installida tarkvara, 0x80cf4017:** Teie konto sert on aegunud. Uuesti laadida PC kliendi tarkvara paketi Intune konsoolis. Läbi selle dokumentatsioonist.
  
 **Tõrkekood 0x801c0003:** Tõrge võib ilmneda järgmistel juhtudel:
  
-  Kasutajal on rohkem kui seadme seadmete. Läbi nende dokumentide [seade eemaldada](https://docs.microsoft.com/intune/devices-wipe) või [muuta seadme piirang](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Kasutajad võivad ühendada seadmeid Azure AD" on seatud "ei ole." Määrata kõigile või kasutajad. Vaadake lisateabe saamiseks [selle dokumentatsiooni](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .

-  Mõni teine kasutaja on juba registreeritud seadme. Kui see juhtub, Eemalda seadme Azure Intune konsooli või käsitsi unenroll seade enne uuesti proovimist.

-  Seade on Windows 10 Home. Ainult Windows 10 Pro, hariduse ja ettevõtluse SKUs saab liituda Azure Active Directory.

Lisaressursse, mis probleemi lahendada:
  
-  Diagnoosimiseks ja lahendamiseks ühise registreerimise rikete [Intune tõrkeotsingu portaali](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) abil. Läbi [selle dokumendi](https://docs.microsoft.com/intune/help-desk-operators) lisateabe saamiseks.

-  Läbi nende dokumentide nimekiri kõige sagedasemad vead, mis takistavad registreerimine ja lahendused igale: [tõrkeotsing juhend](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ja [tõrkeotsing doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Kuidas registreeruda Windowsi seadmetes Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
