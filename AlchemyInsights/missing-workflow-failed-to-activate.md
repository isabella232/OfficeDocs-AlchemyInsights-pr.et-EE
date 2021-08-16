---
title: Töövoogu ei saanud aktiveerida
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: d703e87f355f05bf4a1d71e5daddce96db988380bb48accc81c95f1ba91fbb2b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065424"
---
# <a name="missing-workflow-failed-to-activate"></a>Töövoogu ei saanud aktiveerida

Microsoft SharePoint saidikogumis ei saa loendisse või teeki lisada globaalselt taaskasutatavat töövoogu (nt "Kinnitamine – SharePoint 2010").
  
Selle probleemi lahendamiseks tehke järgmist. 
  
1. Avage saidikogumi juursaidid SharePoint Designer 2013.
  
2. Valige **jaotises Saidiobjektid** **suvand Töövood**. 
  
3. Klõpsake **lindi** Töövood jaotises **Uus** nuppu **Taaskasutatav töövoog**. 
  
4. Sisestage **vormil Create Reusable Workflow** (Taaskasutatava töövoo loomine) nimi ** *Repair2010* **. Klõpsake **jaotises Platvormi** tüüp SharePoint **2010 töövoog** ja seejärel nuppu **OK**. 
  
1. Klõpsake **lindi Töövoog** jaotises **Salvesta** nuppu **Avalda.** 
  
2. Valige **töövoo lindi** jaotises **Haldamine** käsk **Avalda globaalselt**. Klõpsake kuvatavas kinnituse dialoogiboksis nuppu **OK**. 
  
3. Otsige veebibrauseris üles saidikogumi juurveebisaidid ja seejärel juurdepääsege saidile **Sätted** \> **Saidikogumi funktsioonid**. Seejärel lülitage **töövood sisse/ välja.** 
  
· Kui funktsioon on *aktiveeritud,* klõpsake nuppu **Inaktiveeri ja** seejärel nuppu **Aktiveeri.** 
  
· Kui funktsioon on  *inaktiveeritud,*  klõpsake nuppu **Aktiveeri**. 
  
Lisateavet leiate järgmisest [artiklist.](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)
  

