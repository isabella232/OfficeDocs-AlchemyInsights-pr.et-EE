---
title: Windows 10 käivitamise sätted
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
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751131"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="f254a-102">Windows 10 käivitamise sätted</span><span class="sxs-lookup"><span data-stu-id="f254a-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="f254a-103">**Käivitamisel automaatselt käivitatavate rakenduste muutmine**</span><span class="sxs-lookup"><span data-stu-id="f254a-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="f254a-104">Avage [sätted > rakendused > käivitus](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="f254a-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="f254a-105">Veenduge **,** et mõni rakendus, mida soovite käivitamisel käitada, oleks sisse lülitatud.</span><span class="sxs-lookup"><span data-stu-id="f254a-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="f254a-106">**Rakenduse käivitamisel automaatselt käivitumiseks rakenduse lisamine**</span><span class="sxs-lookup"><span data-stu-id="f254a-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="f254a-107">Klõpsake või puudutage nuppu **Käivita** ja otsige üles rakendus, mille soovite käivitada käivitamisel.</span><span class="sxs-lookup"><span data-stu-id="f254a-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="f254a-108">Paremklõpsake rakendust, klõpsake käsku **rohkem**ja seejärel klõpsake käsku **Ava kausta asukoht**.</span><span class="sxs-lookup"><span data-stu-id="f254a-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="f254a-109">Avaneb asukoht, kus rakenduse otsetee on salvestatud.</span><span class="sxs-lookup"><span data-stu-id="f254a-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="f254a-110">Kui fail pole avatud, tähendab see seda, et rakendust ei saa käivitamisel käitada.</span><span class="sxs-lookup"><span data-stu-id="f254a-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="f254a-111">Kui faili asukoht on avatud, vajutage klahvikombinatsiooni **Windowsi logoga klahv + R**, tippige **Shell: Startup**ja seejärel klõpsake nuppu **OK**.</span><span class="sxs-lookup"><span data-stu-id="f254a-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="f254a-112">Avatakse kaust Startup (Startup).</span><span class="sxs-lookup"><span data-stu-id="f254a-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="f254a-113">Kopeerige ja kleepige otsetee rakendusse, mis asub kaustast Startup (käivituskaustas).</span><span class="sxs-lookup"><span data-stu-id="f254a-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="f254a-114">**Täpsemad käivitamise suvandid (sh turvarežiim, UEFI sätted ja teisest seadmest käivitamine)**</span><span class="sxs-lookup"><span data-stu-id="f254a-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="f254a-115">Salvestage oma töö ja sulgege avatud dokumendid, kuna need toimingud taaskäivitavad teie arvuti.</span><span class="sxs-lookup"><span data-stu-id="f254a-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="f254a-116">Avage [sätted > värskenda & turve > taastamine](ms-settings:recovery?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="f254a-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="f254a-117">Klõpsake jaotises **Täpsem käivitamine**nuppu **Taaskäivita kohe**.</span><span class="sxs-lookup"><span data-stu-id="f254a-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="f254a-118">Pärast arvuti taaskäivitamist valige Kuva valik.</span><span class="sxs-lookup"><span data-stu-id="f254a-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="f254a-119">Seadmest (nt USB-draivilt) buutimiseks klõpsake nuppu **Kasuta seadet**.</span><span class="sxs-lookup"><span data-stu-id="f254a-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="f254a-120">UEFI sätete (mõnikord BIOS-i häälestamise) sisestamiseks klõpsake nuppu **tõrkeotsing > Täpsemad suvandid > UEFI püsivara sätted**.</span><span class="sxs-lookup"><span data-stu-id="f254a-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="f254a-121">Turvarežiimi sisestamiseks või täpsemate käivitamise sätete muutmiseks klõpsake nuppu **tõrkeotsing > Täpsemad suvandid > käivitamise sätted**ja seejärel klõpsake nuppu **Taaskäivita**.</span><span class="sxs-lookup"><span data-stu-id="f254a-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="f254a-122">Teil võidakse paluda sisestada [BitLockeri taastevõti](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span><span class="sxs-lookup"><span data-stu-id="f254a-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="f254a-123">Kui teie arvuti taaskäivitub uuesti, klõpsake selle käivitamise säte, mida soovite kasutada.</span><span class="sxs-lookup"><span data-stu-id="f254a-123">After your PC restarts again, click the startup setting you want to use.</span></span>