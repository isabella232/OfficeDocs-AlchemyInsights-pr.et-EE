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
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="04180-102">Windowsi virtuaaltöölaua probleemide tuvastamine</span><span class="sxs-lookup"><span data-stu-id="04180-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="04180-103">Windows Virtual Desktop Diagnostics kasutab ainult ühte PowerShelli cmdlet-käsku, kuid sisaldab mitmeid valikulisi parameetreid, mis aitavad probleeme kitsendada ja isoleerida.</span><span class="sxs-lookup"><span data-stu-id="04180-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="04180-104">Alustamiseks:</span><span class="sxs-lookup"><span data-stu-id="04180-104">To get started:</span></span> 

1. <span data-ttu-id="04180-105">Laadige alla ja importige Windows Virtual Desktop PowerShelli moodul.</span><span class="sxs-lookup"><span data-stu-id="04180-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="04180-106">Lisateavet leiate teemast [Windows PowerShelli Windows Virtual Desktopi cmdlet-käsud.](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)</span><span class="sxs-lookup"><span data-stu-id="04180-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="04180-107">Kontosse sisselogimiseks käivitage järgmine cmdlet-käsk.</span><span class="sxs-lookup"><span data-stu-id="04180-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="04180-108">Näide: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="04180-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="04180-109">**MÄRKUS.** Kõik PowerShelli kasutavad päringud peavad sisaldama kas parameetrit -UserName või -ActivityID.</span><span class="sxs-lookup"><span data-stu-id="04180-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="04180-110">Lisateavet jälgimisvõimaluste kohta leiate teemast [Logianalüüsi kasutamine diagnostikafunktsiooni jaoks.](https://go.microsoft.com/fwlink/?linkid=2126847)</span><span class="sxs-lookup"><span data-stu-id="04180-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="04180-111">Diagnostikategevuste filtreerimiseks kasutaja järgi käivitage järgmine cmdlet-käsk.</span><span class="sxs-lookup"><span data-stu-id="04180-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="04180-112">Näide: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="04180-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="04180-113">Probleemide diagnoosimiseks saate käivitada filtrite loendi.</span><span class="sxs-lookup"><span data-stu-id="04180-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="04180-114">Lisateavet probleemide diagnoosimise kohta leiate teemast Windowsi virtuaaltöölaua [probleemide tuvastamine ja diagnoosimine.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)</span><span class="sxs-lookup"><span data-stu-id="04180-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="04180-115">Levinumate tõrgete kohta leiate lisateavet teemast [Levinud tõrked senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span><span class="sxs-lookup"><span data-stu-id="04180-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
