---
title: 2010. aasta kinnitamise töövoogu ei saa lisada
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: e74c842f8b4be321664f8c2f1f58c570d0724d80edb1264add0647bf313bc82f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020332"
---
# <a name="unable-to-add-2010-approval-workflow"></a>2010. aasta kinnitamise töövoogu ei saa lisada

Microsoft SharePoint saidikogumis ei saa loendisse või teeki lisada globaalselt taaskasutatavat töövoogu (nt "Kinnitamine – SharePoint 2010").
  
Selle probleemi lahendamiseks tehke järgmist. 
  
1. Avage saidikogumi juursaidid SharePoint Designer 2013.
  
2. Valige **jaotises Saidiobjektid** **suvand Töövood**. 
  
3. Klõpsake **lindi** Töövood jaotises **Uus** nuppu **Taaskasutatav töövoog**. 
  
4. Sisestage **vormil Create Reusable Workflow** (Taaskasutatava töövoo loomine) nimi ** *Repair2010* **. Klõpsake **jaotises Platvormi** tüüp SharePoint **2010 töövoog** ja seejärel nuppu **OK**. 
  
1. Klõpsake **lindi Töövoog** jaotises **Salvesta** nuppu **Avalda.** 
  
2. Valige **töövoo lindi** jaotises **Haldamine** käsk **Avalda globaalselt**. Klõpsake kuvatavas kinnituse dialoogiboksis nuppu **OK**. 
  
3. Otsige veebibrauseris üles saidikogumi juurveebisaidid ja seejärel juurdepääsege saidile **Sätted** \> **Saidikogumi funktsioonid**. Lülitage **töövood sisse/välja.** 
  
· Kui funktsioon on *aktiveeritud,* klõpsake nuppu **Inaktiveeri ja** seejärel nuppu **Aktiveeri.** 
  
· Kui funktsioon on  *inaktiveeritud,*  klõpsake nuppu **Aktiveeri**. 
  
Lisateavet leiate järgmisest [artiklist.](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)
  

