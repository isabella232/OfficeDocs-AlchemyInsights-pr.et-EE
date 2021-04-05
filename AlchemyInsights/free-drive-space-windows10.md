---
title: Windows 10 kettaruumi vabastamine
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505352"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="c0c11-102">Windows 10 kettaruumi vabastamine</span><span class="sxs-lookup"><span data-stu-id="c0c11-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="c0c11-103">Siit leiate Windowsis kettaruumi vabastamiseks kaks võimalust.</span><span class="sxs-lookup"><span data-stu-id="c0c11-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="c0c11-104">Vabastage Windows 10 kettaruumi.</span><span class="sxs-lookup"><span data-stu-id="c0c11-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="c0c11-105">Vabastage Windows 10 värskenduste jaoks kettaruumi välise mäluseadme abil.</span><span class="sxs-lookup"><span data-stu-id="c0c11-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="c0c11-106">Kui pärast kettapuhastust on kettaruumi endiselt vähe, võib probleem olla selles, et ajutiste failide kaust Temp täidetakse kiiresti Microsoft Store’i kasutatud rakendusefailidega (.appx).</span><span class="sxs-lookup"><span data-stu-id="c0c11-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="c0c11-107">Probleemi lahendamiseks lähtestage Microsoft Store, tühjendage Microsoft Store’i vahemälu ja seejärel käivitage Windows Update’i tõrkeotsing.</span><span class="sxs-lookup"><span data-stu-id="c0c11-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="c0c11-108">Enne järgmiste toimingute tegemist tuleb Microsoft Store kindlasti sulgeda.</span><span class="sxs-lookup"><span data-stu-id="c0c11-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="c0c11-109">**1. toiming: Microsoft Store’i lähtestamine**</span><span class="sxs-lookup"><span data-stu-id="c0c11-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="c0c11-110">**Märkus** See kustutab seadmest jäädavalt rakenduseandmed (sh eelistused ja sisselogimisandmed).</span><span class="sxs-lookup"><span data-stu-id="c0c11-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="c0c11-111">Valige **Start** > **Sätted** > **Rakendused** > **Rakendused ja funktsioonid**.</span><span class="sxs-lookup"><span data-stu-id="c0c11-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="c0c11-112">Otsige rakenduste loendist üles Microsoft Store ja valige see.</span><span class="sxs-lookup"><span data-stu-id="c0c11-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="c0c11-113">Valige **Täpsemad suvandid**.</span><span class="sxs-lookup"><span data-stu-id="c0c11-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="c0c11-114">Kerige allapoole ja valige **Lähtesta** ja seejärel **kinnitage lähtestamine**.</span><span class="sxs-lookup"><span data-stu-id="c0c11-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="c0c11-115">**2. toiming: Microsoft Store’i vahemälu tühjendamine**</span><span class="sxs-lookup"><span data-stu-id="c0c11-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="c0c11-116">Dialoogiboksi „Käivita“ avamiseks vajutage klahvikombinatsiooni Windowsi logoga klahv + R.</span><span class="sxs-lookup"><span data-stu-id="c0c11-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="c0c11-117">Tippige wsreset.exe ja valige **OK**.</span><span class="sxs-lookup"><span data-stu-id="c0c11-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="c0c11-118">Avaneb tühi käsuviibaaken.</span><span class="sxs-lookup"><span data-stu-id="c0c11-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="c0c11-119">Umbes 10 sekundi pärast sulgub aken automaatselt ja avaneb Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="c0c11-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="c0c11-120">**3. toiming: Windows Update’i lähtestamine**</span><span class="sxs-lookup"><span data-stu-id="c0c11-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="c0c11-121">Valige **Start** > **Sätted** > **Värskendamine ja turvalisus** > **Tõrkeotsing**.</span><span class="sxs-lookup"><span data-stu-id="c0c11-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="c0c11-122">Kerige allapoole ja valige loendist **Windows Update** ning valige **Käivita tõrkeotsing**.</span><span class="sxs-lookup"><span data-stu-id="c0c11-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="c0c11-123">Taaskäivitage arvuti ja kontrollige, kas probleem on lahendatud.</span><span class="sxs-lookup"><span data-stu-id="c0c11-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

