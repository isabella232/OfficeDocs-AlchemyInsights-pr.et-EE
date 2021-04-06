---
title: Windowsi virtuaaltöölaua probleemide tuvastamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595627"
---
# <a name="identify-windows-virtual-desktop-issues"></a>Windowsi virtuaaltöölaua probleemide tuvastamine

Windows Virtual Desktop Diagnostics kasutab ainult ühte PowerShelli cmdlet-käsku, kuid sisaldab mitmeid valikulisi parameetreid, mis aitavad probleeme kitsendada ja isoleerida. Alustamiseks: 

1. Laadige alla ja importige Windows Virtual Desktop PowerShelli moodul. Lisateavet leiate teemast [Windows PowerShelli Windows Virtual Desktopi cmdlet-käsud.](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)

1. Kontosse sisselogimiseks käivitage järgmine cmdlet-käsk.
    
    Näide: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**MÄRKUS.** Kõik PowerShelli kasutavad päringud peavad sisaldama kas parameetrit -UserName või -ActivityID. Lisateavet jälgimisvõimaluste kohta leiate teemast [Logianalüüsi kasutamine diagnostikafunktsiooni jaoks.](https://go.microsoft.com/fwlink/?linkid=2126847)

Diagnostikategevuste filtreerimiseks kasutaja järgi käivitage järgmine cmdlet-käsk.

Näide: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

Probleemide diagnoosimiseks saate käivitada filtrite loendi. Lisateavet probleemide diagnoosimise kohta leiate teemast Windowsi virtuaaltöölaua [probleemide tuvastamine ja diagnoosimine.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)

Levinumate tõrgete kohta leiate lisateavet teemast [Levinud tõrked senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).
