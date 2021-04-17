---
title: Heliprobleemide tõrkeotsing opsüsteemis Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 1bafc97b2ab1394087d2451d73168a29267d64ab
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833287"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="63c43-102">Heliprobleemide tõrkeotsing opsüsteemis Windows 10</span><span class="sxs-lookup"><span data-stu-id="63c43-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="63c43-103">**Helitõrkeotsija käivitamine**</span><span class="sxs-lookup"><span data-stu-id="63c43-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="63c43-104">Avage [tõrkeotsing.](ms-settings:troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="63c43-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="63c43-105">Valige **Esita**  >  **heli. Käivitage tõrkeotsija.**</span><span class="sxs-lookup"><span data-stu-id="63c43-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="63c43-106">**Vaikeseadme seadis**</span><span class="sxs-lookup"><span data-stu-id="63c43-106">**Set the default device**</span></span>

<span data-ttu-id="63c43-107">Kui loote usb- või HDMI-seadme abil ühenduse heliseadmega, peate võib-olla selle seadme vaikeseadmeks häälestama.</span><span class="sxs-lookup"><span data-stu-id="63c43-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="63c43-108">Avage **Start**  >  **Sound**(Käivita heli) ja seejärel valige **tulemite loendist** Heli või Muuda süsteemi helisid. </span><span class="sxs-lookup"><span data-stu-id="63c43-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="63c43-109">Valige **vahekaardil Taasesitus** soovitud seade, valige **Sea vaikesäte** ja seejärel valige **OK**.</span><span class="sxs-lookup"><span data-stu-id="63c43-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="63c43-110">**Kaablite, helitugevuse, kõlarite ja kõrvaklappide kontrollimine**</span><span class="sxs-lookup"><span data-stu-id="63c43-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="63c43-111">Kontrollige kõlarite ja kõrvaklappide ühendusi lahtiste kaablite kohta ning veenduge, et need on ühendatud õige pistikupesaga.</span><span class="sxs-lookup"><span data-stu-id="63c43-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="63c43-112">Kontrollige oma toite- ja helitugevuse taset ning proovige kõik helitugevuse juhtelemendid üles muuta.</span><span class="sxs-lookup"><span data-stu-id="63c43-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="63c43-113">Mõnel kõlaritel ja rakendustel on oma helitugevuse juhtelemendid. Võimalik, et peate neid kõiki kontrollima, et veenduda, et need on õigetel tasemetel.</span><span class="sxs-lookup"><span data-stu-id="63c43-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="63c43-114">Proovige luua ühendus muu USB-pordi abil.</span><span class="sxs-lookup"><span data-stu-id="63c43-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="63c43-115">**Märkus.** Pidage meeles, et kõlarid ei pruugi töötada, kui kõrvaklapid on ühendatud.</span><span class="sxs-lookup"><span data-stu-id="63c43-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="63c43-116">**Seadmehalduri kontrollimine**</span><span class="sxs-lookup"><span data-stu-id="63c43-116">**Check Device Manager**</span></span>

<span data-ttu-id="63c43-117">Veendumaks, et draiverid on ajased:</span><span class="sxs-lookup"><span data-stu-id="63c43-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="63c43-118">Valige **Start**, tippige **Seadmehaldur** ja **seejärel** valige tulemite loendist Seadmehaldur.</span><span class="sxs-lookup"><span data-stu-id="63c43-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="63c43-119">Valige **jaotises Heli-, video- ja mängukontrollerid** oma helikaart, avage see, valige vahekaart **Draiver** ja valige **Värskenda draiver**.</span><span class="sxs-lookup"><span data-stu-id="63c43-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="63c43-120">**Märkus.** Kui Windows ei leia uut draiverit, otsige seda seadme tootja veebisaidilt ja järgige nende juhiseid.</span><span class="sxs-lookup"><span data-stu-id="63c43-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="63c43-121">**Draiveri uuesti installimine**</span><span class="sxs-lookup"><span data-stu-id="63c43-121">**Reinstall the driver**</span></span>

<span data-ttu-id="63c43-122">Kui te ei saa värskendada Seadmehalduri kaudu või leida tootja veebisaidilt uut draiverit, tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="63c43-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="63c43-123">Paremklõpsake (või vajutage pikalt) seadmehalduris helidraiverit ja valige **Desinstalli**.</span><span class="sxs-lookup"><span data-stu-id="63c43-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="63c43-124">Taaskäivitage seade ja Windows proovib draiveri uuesti installida.</span><span class="sxs-lookup"><span data-stu-id="63c43-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="63c43-125">Kui draiveri uuesti installimine ei tööta, proovige kasutada Windowsiga kaasas olnud üldist helidraiverit.</span><span class="sxs-lookup"><span data-stu-id="63c43-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="63c43-126">Paremklõpsake seadmehalduris (või vajutage pikalt) oma helidraiverit > **Draiveritarkvara** värskendamine Draiveritarkvara sirvimine. Lubage mul valida oma arvuti seadmedraiverite loendist, valige  >    >  High Definition **Audio Device**(Kõrglahutusega heliseade), valige **Edasi** ja järgige installimise juhiseid.</span><span class="sxs-lookup"><span data-stu-id="63c43-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
