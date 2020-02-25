---
title: Bluetoothi probleemide lahendamine Windows 10-s
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: 94dda7a42632f57ce3aef5f467b87df1033b8d49
ms.sourcegitcommit: 9a35768444824cde9e192f1d9daafc9157437244
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/25/2020
ms.locfileid: "42268594"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="6fb22-102">Bluetoothi probleemide lahendamine Windows 10-s</span><span class="sxs-lookup"><span data-stu-id="6fb22-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="6fb22-103">Kui Bluetoothi ikoon puudub või Bluetoothi ei saa sisse või välja lülitada, võiksite käivitada Bluetoothi tõrkeotsingu.</span><span class="sxs-lookup"><span data-stu-id="6fb22-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="6fb22-104">[Avage sätete tõrkeotsing](ms-settings:troubleshoot), klõpsake **Bluetooth** all **leida ja lahendada muid probleeme**, klõpsake nuppu **Käivita tõrkeotsing**.</span><span class="sxs-lookup"><span data-stu-id="6fb22-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="6fb22-105">Kui te ei näe Bluetoothi ikooni, kuid Bluetooth kuvatakse Seadmehalduris:</span><span class="sxs-lookup"><span data-stu-id="6fb22-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="6fb22-106">Klõpsake Seadmehalduris **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="6fb22-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="6fb22-107">Vajutage pikalt (või paremklõpsake) Bluetooth-adapteri nime ja klõpsake **desinstalli seade**.</span><span class="sxs-lookup"><span data-stu-id="6fb22-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="6fb22-108">Sulgege Windowsi seade, oodake mõni sekund ja seejärel lülitage see uuesti sisse.</span><span class="sxs-lookup"><span data-stu-id="6fb22-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="6fb22-109">Windows proovib draiverit uuesti installida.</span><span class="sxs-lookup"><span data-stu-id="6fb22-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="6fb22-110">Kui installisite hiljuti Windows 10 värskendusi või täiendasite Windows 10-sse, võiksite kontrollida draiverivärskendusi.</span><span class="sxs-lookup"><span data-stu-id="6fb22-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="6fb22-111">Seadmehalduris klõpsake **Bluetoothi**ja seejärel klõpsake Bluetoothi adapteri nime (mis võib sisaldada sõna "raadio").</span><span class="sxs-lookup"><span data-stu-id="6fb22-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="6fb22-112">Vajutage pikalt (või paremklõpsake) Bluetooth-adapterit ja seejärel klõpsake **Värskenda draiveri** > **Otsing automaatselt värskendatud draiveritarkvara**.</span><span class="sxs-lookup"><span data-stu-id="6fb22-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="6fb22-113">Järgige juhiseid ja seejärel klõpsake nuppu **Sule**.</span><span class="sxs-lookup"><span data-stu-id="6fb22-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="6fb22-114">Kui Windows ei leia uut Bluetoothi draiverit, külastage arvuti tootja veebisaiti ja laadige sealt alla uusim Bluetoothi draiver.</span><span class="sxs-lookup"><span data-stu-id="6fb22-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="6fb22-115">Pärast selle allalaadimist klõpsake nuppu **Värskenda draiverit** > **Sirvi minu arvuti draiveri tarkvara** > **sirvida** asukohta, kus draiverifailid on salvestatud > **OK** > **Järgmine**ja järgige installimiseks juhiseid.</span><span class="sxs-lookup"><span data-stu-id="6fb22-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="6fb22-116">Pärast värskendatud draiveri installimist taaskäivitage arvuti ja seejärel kontrollige, kas see lahendab ühenduse probleemi.</span><span class="sxs-lookup"><span data-stu-id="6fb22-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="6fb22-117">Lisateabe saamiseks Bluetoothi probleemide tõrkeotsingu kohta lugege kogu artiklit, [parandage Bluetoothi probleemid operatsioonisüsteemis Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="6fb22-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
