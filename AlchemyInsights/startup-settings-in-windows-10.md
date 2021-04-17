---
title: Windows 10 käivitussätted
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
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828148"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="ab1e0-102">Windows 10 käivitussätted</span><span class="sxs-lookup"><span data-stu-id="ab1e0-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="ab1e0-103">**Käivituse ajal automaatselt käivituvate rakenduste muutmine**</span><span class="sxs-lookup"><span data-stu-id="ab1e0-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="ab1e0-104">Avage [Sätted > Rakendused > Käivitus](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="ab1e0-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="ab1e0-105">Veenduge, et iga rakendus, mida soovite käivitamisel käitada, oleks sisse **lülitatud.**</span><span class="sxs-lookup"><span data-stu-id="ab1e0-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="ab1e0-106">**Rakenduse lisamine käivitumiseks automaatselt käivitamisel**</span><span class="sxs-lookup"><span data-stu-id="ab1e0-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="ab1e0-107">Klõpsake või **puudutage nuppu Start** ja otsige üles rakendus, mida soovite käivitamisel käivitada.</span><span class="sxs-lookup"><span data-stu-id="ab1e0-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="ab1e0-108">Paremklõpsake rakendust, klõpsake käsku **Rohkem** ja seejärel klõpsake käsku **Ava faili asukoht.**</span><span class="sxs-lookup"><span data-stu-id="ab1e0-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="ab1e0-109">See avab asukoha, kuhu rakenduse otsetee salvestatakse.</span><span class="sxs-lookup"><span data-stu-id="ab1e0-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="ab1e0-110">Kui faili asukoha avamiseks pole valikut, tähendab see, et rakendust ei saa käivitamisel käivitada.</span><span class="sxs-lookup"><span data-stu-id="ab1e0-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="ab1e0-111">Kui faili asukoht on avatud, vajutage klahvikombinatsiooni **Windowsi logoga klahv + R**, tippige **shell:startup** ja seejärel klõpsake nuppu **OK**.</span><span class="sxs-lookup"><span data-stu-id="ab1e0-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="ab1e0-112">Avatakse käivituskaust.</span><span class="sxs-lookup"><span data-stu-id="ab1e0-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="ab1e0-113">Kopeerige ja kleepige rakenduse otsetee faili asukohast käivituskausta.</span><span class="sxs-lookup"><span data-stu-id="ab1e0-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="ab1e0-114">**Täpsemad käivitussuvandid (sh turvarežiim, UEFI sätted ja käivitamine teisest seadmest)**</span><span class="sxs-lookup"><span data-stu-id="ab1e0-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="ab1e0-115">Salvestage oma töö ja sulgege kõik avatud dokumendid, kuna need toimingud taaskäivitavad teie arvuti.</span><span class="sxs-lookup"><span data-stu-id="ab1e0-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="ab1e0-116">Avage [Sätted > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="ab1e0-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="ab1e0-117">Klõpsake **jaotises Täpsem käivitus** nuppu Taaskäivita **kohe**.</span><span class="sxs-lookup"><span data-stu-id="ab1e0-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="ab1e0-118">Pärast arvuti taaskäivitamist kuvale Suvandi valimine tehke valik.</span><span class="sxs-lookup"><span data-stu-id="ab1e0-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="ab1e0-119">Seadmest (nt USB-draivilt) algkäivituseks klõpsake **nuppu Kasuta seadet**.</span><span class="sxs-lookup"><span data-stu-id="ab1e0-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="ab1e0-120">UEFI sätete (mõnikord nimetatakse seda ka BIOS-i häälestuseks) sisestamiseks klõpsake **> Täpsemad suvandid > UEFI püsivarasätted**.</span><span class="sxs-lookup"><span data-stu-id="ab1e0-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="ab1e0-121">Turvarežiimi sisenemiseks või täpsemate käivitussätete muutmiseks klõpsake nuppu **Tõrkeotsing > Täpsemad suvandid >** Ja seejärel klõpsake nuppu **Taaskäivita**.</span><span class="sxs-lookup"><span data-stu-id="ab1e0-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="ab1e0-122">Teil võidakse paluda sisestada [BitLockeri taastevõti.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)</span><span class="sxs-lookup"><span data-stu-id="ab1e0-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="ab1e0-123">Pärast arvuti taaskäivitamist klõpsake käivitussätet, mida soovite kasutada.</span><span class="sxs-lookup"><span data-stu-id="ab1e0-123">After your PC restarts again, click the startup setting you want to use.</span></span>