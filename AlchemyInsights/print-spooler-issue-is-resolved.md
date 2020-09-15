---
title: Prindispuuleri probleemi lahendamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 66b39434ef6f9ad2b8392f811704e67c1bcffd2b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801837"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="e9add-102">Prindispuuleri probleemi lahendamine</span><span class="sxs-lookup"><span data-stu-id="e9add-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="e9add-103">Kui teie seadmesse on uuendatud Windows 10  **OS järk 19041,329**, on võimalik, et olete täheldanud probleemi, mille korral teatud printerid ei prindi.</span><span class="sxs-lookup"><span data-stu-id="e9add-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="e9add-104">Prindispuuler võib printimise katsel tõrke või ootamatult sulguda, kuid see ei pärine enam mõjutatud printerist.</span><span class="sxs-lookup"><span data-stu-id="e9add-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="e9add-105">See probleem on lahendatud opsüsteemis OS järk  **19041,331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="e9add-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="e9add-106">**Käimasolev uurimine**</span><span class="sxs-lookup"><span data-stu-id="e9add-106">**Ongoing investigation**</span></span>

<span data-ttu-id="e9add-107">Kohaliku julgeolekuasutuse alamsüsteemi teenuse (LSASS) fail (**Isass.exe**) võib teatud seadmetes nurjuda, kuna tõrketeade "kriitiline süsteem, C:\WINDOWS\system32\Isass.exe, nurjus olekukood c0000008.</span><span class="sxs-lookup"><span data-stu-id="e9add-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="e9add-108">Arvuti tuleb nüüd taaskäivitada ".</span><span class="sxs-lookup"><span data-stu-id="e9add-108">The machine must now be restarted".</span></span>  <span data-ttu-id="e9add-109">**Microsoft töötab eraldusvõimega ja annab eelseisval väljalaskel värskenduse.**</span><span class="sxs-lookup"><span data-stu-id="e9add-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="e9add-110">Lisateavet leiate teemast  [Windows 10 versiooni 2004 teadaolevad probleemid](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="e9add-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>