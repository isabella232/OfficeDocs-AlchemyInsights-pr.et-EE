---
title: Windows 10 kõvakettaruumi vabastamine
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
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035667"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="92164-102">Windows 10 kõvakettaruumi vabastamine</span><span class="sxs-lookup"><span data-stu-id="92164-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="92164-103">Windowsi kettaruumi vabastamiseks on kaks võimalust.</span><span class="sxs-lookup"><span data-stu-id="92164-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="92164-104">Vabastage Windows 10 kõvakettaruumi.</span><span class="sxs-lookup"><span data-stu-id="92164-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="92164-105">Vabastage ruumi Windows 10 värskenduste jaoks välise mäluseadme abil.</span><span class="sxs-lookup"><span data-stu-id="92164-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="92164-106">Kui teil on pärast kettapuhastuse kasutamist endiselt väike kettaruum, on võimalik, et teie temp-kaust täidab kiiresti rakenduse (. appx) failid, mida Microsoft Store kasutab.</span><span class="sxs-lookup"><span data-stu-id="92164-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="92164-107">Probleemi lahendamiseks lähtestage pood, tühjendage ruut Talleta vahemälu ja seejärel käivitage Windows Update ' i tõrkeotsija.</span><span class="sxs-lookup"><span data-stu-id="92164-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="92164-108">Enne nende toimingute jätkamist veenduge, et Microsoft Store oleks suletud.</span><span class="sxs-lookup"><span data-stu-id="92164-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="92164-109">**1. juhis: Microsoft Store ' i lähtestamine**</span><span class="sxs-lookup"><span data-stu-id="92164-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="92164-110">**Märkus** See kustutab seadmest jäädavalt rakenduse andmed, sh teie eelistused ja sisselogimise üksikasjad.</span><span class="sxs-lookup"><span data-stu-id="92164-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="92164-111">Valige menüü **Start**  >  **sätted**  >  **rakendused**  >  **& funktsioonid**.</span><span class="sxs-lookup"><span data-stu-id="92164-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="92164-112">Otsige rakenduste loendist üles ja valige Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="92164-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="92164-113">Valige **Täpsemad suvandid**.</span><span class="sxs-lookup"><span data-stu-id="92164-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="92164-114">Kerige allapoole ja valige **Lähtesta** ja seejärel **kinnitage lähtestamine**.</span><span class="sxs-lookup"><span data-stu-id="92164-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="92164-115">**2. juhis: Microsoft Store ' i vahemälu tühjendamine**</span><span class="sxs-lookup"><span data-stu-id="92164-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="92164-116">Vajutage klahvikombinatsiooni Windowsi logoga klahv + R, et avada dialoogiboks Käivita.</span><span class="sxs-lookup"><span data-stu-id="92164-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="92164-117">Tippige wsreset.exe ja klõpsake **nuppu OK**.</span><span class="sxs-lookup"><span data-stu-id="92164-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="92164-118">Avaneb tühja käsuviiba aken.</span><span class="sxs-lookup"><span data-stu-id="92164-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="92164-119">Umbes 10 sekundi pärast sulgub aken ja pood avaneb automaatselt.</span><span class="sxs-lookup"><span data-stu-id="92164-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="92164-120">**3. juhis: Windows Update ' i lähtestamine**</span><span class="sxs-lookup"><span data-stu-id="92164-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="92164-121">Valige käsk **Alusta**  >  **sätteid**  >  **Värskenda & turvalisuse**  >  **tõrkeotsing**.</span><span class="sxs-lookup"><span data-stu-id="92164-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="92164-122">Liikuge kerides allapoole ja valige loendist **Windows Update** ja valige käsk **Käivita tõrkeotsija**.</span><span class="sxs-lookup"><span data-stu-id="92164-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="92164-123">Taaskäivitage arvuti ja kontrollige, kas teil on endiselt probleeme.</span><span class="sxs-lookup"><span data-stu-id="92164-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

