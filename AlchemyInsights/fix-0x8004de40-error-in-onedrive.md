---
title: Fix 0x8004de40 tõrge OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716024"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Fix 0x8004de40 tõrge OneDrive

Kui saate tõrketeate 0x8004de40 OneDrive ' iga:

- Taaskäivitage mõjutatud arvuti ajal, mis on ühendatud teie Võimeve Directory domeeniga.
- Kui reboot ei lahenda probleemi, lahti ühendada ja ühendada oma seadme Azure AD. 

**Märkus**: sa peaksid olema oma ettevõtte võrgus, tehes neid samme. Ärge tehke neid samme, kui te ei saa luua ühendust oma ettevõtte infrastruktuuriga (nt reisil olles). 

- Avage administraatoriõigustega Käsuviip. 
- Laiendatud käsuviiba avamiseks klõpsake- **Start**, paremklõpsake **Käsuviip**ja seejärel klõpsake nuppu **Käivita administraatorina**.
- Tippige *dsregcmd/Leave* ja vajutage sisestusklahvi **Enter**.
- Kui olete valmis, tippige *dsregcmd/JOIN* ja vajutage sisestusklahvi **Enter**.
- Kui olete valmis, sulgege Käsuviip.
- Taaskäivitage arvuti ja logige OneDrive ' i sisse.