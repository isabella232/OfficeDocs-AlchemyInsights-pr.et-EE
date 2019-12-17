---
title: Fix 0x8004de40 tõrge OneDrive
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052033"
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