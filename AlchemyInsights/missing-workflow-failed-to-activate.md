---
title: Töövoo puudub aktiveerimine nurjus
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 2598111005c219c398b63ca374e8e99348efc02c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762097"
---
# <a name="missing-workflow-failed-to-activate"></a>Töövoo puudub aktiveerimine nurjus

Microsoft SharePointi saidikogumi, ei saa lisada globaalselt korduvkasutatav töövoog (nt "kinnitamine-SharePoint 2010") loendisse või teeki.
  
Selle probleemi lahendamiseks toimige järgmiselt. 
  
1. Avage saidikogumi juursait SharePoint Designer 2013.
  
2. Valige jaotises **saidi objektid** **töövoogude**. 
  
3. Valige lindi **töövoogude** **Uus** jaotis **korduvkasutatav töövoog**. 
  
4. Sisestage vormil **Loo korduvkasutatav töövoog** nimi * * *Repair2010* * *. **Platvormi tüüp**, klõpsake **SharePoint 2010 töövooja**seejärel klõpsake nuppu **OK**. 
  
1. **Töövoo** lindi jaotises **Salvesta** , valige **Avalda**. 
  
2. **Töövoo** lindi jaotises **Halda** valige **Avalda globaalselt**. Valige kuvatavas kinnitusdialoogiboksis nupp **OK**. 
  
3. Veebibrauseri, leidke saidikogumi root kodulehel ja seejärel juurdepääsu **saidi sätted** \> **saidikogumi funktsioonid**. Seejärel lülitage **töövoogude** funktsioon: 
  
· Kui funktsioon on *aktiveeritud* , klõpsake nuppu **Desaktiveeri** ja seejärel nuppu **Aktiveeri**. 
  
· Kui funktsioon on *desaktiveeritud* , klõpsake nuppu **Aktiveeri**. 
  
Lisateabe saamiseks lugege järgmist [artiklit](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

