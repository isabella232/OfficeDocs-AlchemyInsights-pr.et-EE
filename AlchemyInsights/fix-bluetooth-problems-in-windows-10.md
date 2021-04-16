---
title: Bluetoothi probleemide lahendamine opsüsteemis Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: f20bf4a642e019c7901e988a027e0220f0f1b07b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812928"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="75d7a-102">Bluetoothi probleemide lahendamine opsüsteemis Windows 10</span><span class="sxs-lookup"><span data-stu-id="75d7a-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="75d7a-103">Kui Bluetoothi ikoon puudub või Bluetoothi ei saa sisse või välja lülitada, võite käivitada Bluetoothi tõrkeotsija.</span><span class="sxs-lookup"><span data-stu-id="75d7a-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="75d7a-104">[Avage tõrkeotsing , klõpsake jaotises](ms-settings:troubleshoot)Muude probleemide **otsija ja lahendamine** nuppu **Bluetooth** ja seejärel käsku **Käivita tõrkeotsija.**</span><span class="sxs-lookup"><span data-stu-id="75d7a-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="75d7a-105">Kui Bluetoothi ikooni ei kuvata, kuid Bluetooth kuvatakse seadmehalduris.</span><span class="sxs-lookup"><span data-stu-id="75d7a-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="75d7a-106">Klõpsake seadmehalduris nuppu **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="75d7a-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="75d7a-107">Vajutage pikalt (või paremklõpsake) Bluetoothi adapteri nime ja klõpsake käsku **Desinstalli seade.**</span><span class="sxs-lookup"><span data-stu-id="75d7a-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="75d7a-108">Sulgege Oma Windowsi seade, oodake paar sekundit ja seejärel lülitage see uuesti sisse.</span><span class="sxs-lookup"><span data-stu-id="75d7a-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="75d7a-109">Windows proovib draiveri uuesti installida.</span><span class="sxs-lookup"><span data-stu-id="75d7a-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="75d7a-110">Kui olete windows 10 värskendused hiljuti installinud või windows 10 kasutusele võtnud, võite draiverivärskendusi kontrollida.</span><span class="sxs-lookup"><span data-stu-id="75d7a-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="75d7a-111">Klõpsake seadmehalduris **nuppu Bluetooth** ja seejärel bluetoothi adapteri nime (mis võib sisaldada sõna "raadio").</span><span class="sxs-lookup"><span data-stu-id="75d7a-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="75d7a-112">Vajutage pikalt (või paremklõpsake) Bluetoothi adapterit ja seejärel klõpsake värskendatud **draiveritarkvara** otsimiseks  >  **nuppu Värskenda draiveriotsing automaatselt.**</span><span class="sxs-lookup"><span data-stu-id="75d7a-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="75d7a-113">Järgige juhiseid ja seejärel klõpsake nuppu **Sule.**</span><span class="sxs-lookup"><span data-stu-id="75d7a-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="75d7a-114">Kui Windows ei leia uut Bluetoothi draiverit, külastage arvuti tootja veebisaiti ja laadige sealt alla uusim Bluetooth-draiver.</span><span class="sxs-lookup"><span data-stu-id="75d7a-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="75d7a-115">Kui olete draiveri alla laadinud, klõpsake nuppu **Värskenda** draiverit Draiveritarkvara sirvimine Sirvige asukohta, kuhu draiverifailid on talletatud > OK Järgmine , ja järgige  >    >     >  installimiseks juhiseid.</span><span class="sxs-lookup"><span data-stu-id="75d7a-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="75d7a-116">Pärast värskendatud draiveri installimist taaskäivitage seade ja kontrollige, kas see lahendab ühendusprobleemi.</span><span class="sxs-lookup"><span data-stu-id="75d7a-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="75d7a-117">Lisateavet Bluetoothi probleemide tõrkeotsingu kohta leiate artiklist Bluetoothi probleemide lahendamine [opsüsteemis Windows 10.](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems)</span><span class="sxs-lookup"><span data-stu-id="75d7a-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
