---
title: Bluetooth-probleemide lahendamine opsüsteemis Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: 7e7a397a1f6777972a81bcbb6bffa1c98d8370a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730155"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="cb379-102">Bluetooth-probleemide lahendamine opsüsteemis Windows 10</span><span class="sxs-lookup"><span data-stu-id="cb379-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="cb379-103">Kui Bluetoothi ikoon on puudu või Bluetoothi ei saa sisse või välja lülitada, võite kasutada Bluetoothi tõrkeotsijat.</span><span class="sxs-lookup"><span data-stu-id="cb379-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="cb379-104">[Avage tõrkeotsingu sätted](ms-settings:troubleshoot), klõpsake jaotises **Otsi ja paranda muid probleeme**nuppu **Bluetooth** , klõpsake nuppu **Käivita tõrkeotsija**.</span><span class="sxs-lookup"><span data-stu-id="cb379-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="cb379-105">Kui te ei näe Bluetoothi ikooni, kuid Bluetooth kuvatakse Seadmehalduris.</span><span class="sxs-lookup"><span data-stu-id="cb379-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="cb379-106">Klõpsake Seadmehalduris nuppu **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="cb379-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="cb379-107">Vajutage pikalt (või paremklõpsake) Bluetoothi adapteri nime ja seejärel klõpsake käsku **desinstalli seade**.</span><span class="sxs-lookup"><span data-stu-id="cb379-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="cb379-108">Sulgege Windowsi seade, oodake mõni sekund ja seejärel lülitage see uuesti välja.</span><span class="sxs-lookup"><span data-stu-id="cb379-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="cb379-109">Windows proovib draiveri uuesti installida.</span><span class="sxs-lookup"><span data-stu-id="cb379-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="cb379-110">Kui installisite hiljuti Windows 10 värskendusi või täiendasite versioonile Windows 10, võite kontrollida draiveri värskendusi.</span><span class="sxs-lookup"><span data-stu-id="cb379-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="cb379-111">Seadmehalduris valige **Bluetooth**ja seejärel klõpsake Bluetoothi adapteri nime (mis võib sisaldada sõna "raadio").</span><span class="sxs-lookup"><span data-stu-id="cb379-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="cb379-112">Vajutage pikalt (või paremklõpsake) Bluetoothi adapterit ja seejärel klõpsake käsku **Värskenda draiverit**  >  **automaatselt värskendatud draiveri tarkvara jaoks**.</span><span class="sxs-lookup"><span data-stu-id="cb379-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="cb379-113">Järgige juhiseid ja seejärel klõpsake nuppu **Sule**.</span><span class="sxs-lookup"><span data-stu-id="cb379-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="cb379-114">Kui Windows ei leia uut Bluetoothi draiverit, külastage arvuti tootja veebisaiti ja laadige sealt alla uusim Bluetooth-draiver.</span><span class="sxs-lookup"><span data-stu-id="cb379-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="cb379-115">Kui olete selle alla laadinud, klõpsake draiveri tarkvara Sirvi **draiveri**  >  **sirvimiseks draiveri tarkvara sirvige**  >  **Browse** asukohta, kus draiveri failid on talletatud > **OK**  >  **Next**, ja järgige installimise juhiseid.</span><span class="sxs-lookup"><span data-stu-id="cb379-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="cb379-116">Pärast värskendatud draiveri installimist taaskäivitage arvuti ja kontrollige, kas see lahendab ühendusega seotud probleemi.</span><span class="sxs-lookup"><span data-stu-id="cb379-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="cb379-117">Lisateavet Bluetoothi probleemide tõrkeotsingu kohta leiate artiklist täielik artikkel, [Windows 10 Bluetoothi probleemide lahendamine](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="cb379-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
