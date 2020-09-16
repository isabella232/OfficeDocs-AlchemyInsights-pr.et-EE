---
title: Windows 10 heliga seotud probleemide tõrkeotsing
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
- "3476"
- "9001463"
ms.openlocfilehash: 88157f9c82bc970e989d47f5cf376b7ce485cb2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750303"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="1432b-102">Windows 10 heli probleemide tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="1432b-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="1432b-103">**Heli tõrkeotsija käivitamine**</span><span class="sxs-lookup"><span data-stu-id="1432b-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="1432b-104">Avage [tõrkeotsingu sätted](ms-settings:troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="1432b-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="1432b-105">Klõpsake nuppu **Esita heli**  >  **ja käivitage tõrkeotsija**.</span><span class="sxs-lookup"><span data-stu-id="1432b-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="1432b-106">**Vaike-seadme määramine**</span><span class="sxs-lookup"><span data-stu-id="1432b-106">**Set the default device**</span></span>

<span data-ttu-id="1432b-107">Kui loote ühenduse USB-või HDMI-kaabli abil, peate võib-olla seadma selle seadme vaikeprogrammiks.</span><span class="sxs-lookup"><span data-stu-id="1432b-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="1432b-108">Avage nupp **Käivita**  >  **heli**ja valige tulemite loendist **heli** või **Muuda süsteemi helisid** .</span><span class="sxs-lookup"><span data-stu-id="1432b-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="1432b-109">Valige vahekaardil **taasesitus** soovitud seade, valige **Määra vaikesätted**ja seejärel klõpsake **nuppu OK**.</span><span class="sxs-lookup"><span data-stu-id="1432b-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="1432b-110">**Kaablite, helitugevuse, kõlarite ja kõrvaklappide kontrollimine**</span><span class="sxs-lookup"><span data-stu-id="1432b-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="1432b-111">Kontrollige, kas kõlarite ja kõrvaklappide ühendused on lahtised kaablid, ja veenduge, et need on ühendatud õige Jackiga.</span><span class="sxs-lookup"><span data-stu-id="1432b-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="1432b-112">Kontrollige oma võimsuse ja helitugevuse taset ning proovige kõik helitugevuse juhtelemendid üles keerata.</span><span class="sxs-lookup"><span data-stu-id="1432b-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="1432b-113">Mõnedel kõlaritel ja rakendustel on oma helitugevuse juhtelemendid; võimalik, et peate need kõik üle vaatama, et veenduda, kas need on õigel tasemel.</span><span class="sxs-lookup"><span data-stu-id="1432b-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="1432b-114">Proovige ühendust luua mõne muu USB-pordi kaudu.</span><span class="sxs-lookup"><span data-stu-id="1432b-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="1432b-115">**Märkus**: Pidage meeles, et kõlarid ei pruugi töötada, kui kõrvaklapid on ühendatud.</span><span class="sxs-lookup"><span data-stu-id="1432b-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="1432b-116">**Seadmehalduri kontrollimine**</span><span class="sxs-lookup"><span data-stu-id="1432b-116">**Check Device Manager**</span></span>

<span data-ttu-id="1432b-117">Et veenduda, kas draiverid on värskendatud, tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="1432b-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="1432b-118">Valige nupp **Start**, tippige **Seadmehaldur**ja seejärel valige tulemite loendist **Seadmehaldur** .</span><span class="sxs-lookup"><span data-stu-id="1432b-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="1432b-119">Valige jaotises **heli-, video-ja mängukontrollerid**oma helikaart, avage see, valige vahekaart draiver ja klõpsake nuppu **draiveri** **värskendamine**.</span><span class="sxs-lookup"><span data-stu-id="1432b-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="1432b-120">**Märkus**: kui Windows uut draiverit ei leia, otsige seda seadme tootja veebisaidilt ja järgige juhiseid.</span><span class="sxs-lookup"><span data-stu-id="1432b-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="1432b-121">**Draiveri uuesti installimine**</span><span class="sxs-lookup"><span data-stu-id="1432b-121">**Reinstall the driver**</span></span>

<span data-ttu-id="1432b-122">Kui te ei saa värskendada Device Manageri kaudu või leida tootja veebisaidilt uut draiverit, proovige järgmisi toiminguid.</span><span class="sxs-lookup"><span data-stu-id="1432b-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="1432b-123">Seadmehalduris Paremklõpsake (või vajutage pikalt) heli draiverit ja valige **Uninstall (Desinstalli**).</span><span class="sxs-lookup"><span data-stu-id="1432b-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="1432b-124">Taaskäivitage oma seade ja Windows proovib draiveri uuesti installida.</span><span class="sxs-lookup"><span data-stu-id="1432b-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="1432b-125">Kui draiveri uuesti installimine ei toimi, proovige kasutada Windowsiga kaasas olevat üldist heli draiverit.</span><span class="sxs-lookup"><span data-stu-id="1432b-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="1432b-126">Seadmehalduris Paremklõpsake (või vajutage pikalt) oma heliriistvara > draiveri **tarkvara**  >  **sirvimine minu arvuti draiveri tarkvara jaoks**  >  , kui valite**minu arvutis seadmedraiverid**, valige **kõrglahutusega heliseade**, klõpsake nuppu **edasi**ja järgige juhiseid selle installimiseks.</span><span class="sxs-lookup"><span data-stu-id="1432b-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
