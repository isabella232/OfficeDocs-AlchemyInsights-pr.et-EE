---
title: Fix 0x8004de40 tõrge OneDrive ' is
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755844"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Fix 0x8004de40 tõrge OneDrive ' is

Kui saate tõrketeate 0x8004de40 OneDrive:

- Taaskäivitage mõjutatud arvuti ajal, mis on ühendatud teie Võimeve Directory domeeniga.
- Kui reboot ei lahenda probleemi, lahti ühendada ja ühendada oma seadme Azure AD. 

**Märkus**: sa peaksid olema oma ettevõtte võrgus, tehes neid samme. Ärge tehke neid samme, kui te ei saa luua ühendust oma ettevõtte infrastruktuuriga (nt reisil olles). 

- Avage administraatoriõigustega Käsuviip. 
- Laiendatud käsuviiba avamiseks klõpsake- **Start**, paremklõpsake **Käsuviip**ja seejärel klõpsake nuppu **Käivita administraatorina**.
- Tippige *dsregcmd/Leave* ja vajutage sisestusklahvi **Enter**.
- Kui olete valmis, tippige *dsregcmd/JOIN* ja vajutage sisestusklahvi **Enter**.
- Kui olete valmis, sulgege Käsuviip.
- Taaskäivitage arvuti ja logige OneDrive ' i sisse.