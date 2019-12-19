---
title: Olemasoleva kuvari tõrkeotsing
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: d90baddd01bdf8508bd6289509c8399b8241887a
ms.sourcegitcommit: 42463e8d8869f36225a27388d83d37629c6b149e
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/18/2019
ms.locfileid: "40738565"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="95919-102">Olemasoleva kuvari tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="95919-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="95919-103">Proovige neid lahendusi kuvari tõrkeotsinguks.</span><span class="sxs-lookup"><span data-stu-id="95919-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="95919-104">**Värskenda kuvari Kuva:**</span><span class="sxs-lookup"><span data-stu-id="95919-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="95919-105">Vajutage samal ajal järgmisi klahve: Windowsi klahv + CTRL + SHIFT + B. See värskendab suhtlust teie graafikadraiveriga.</span><span class="sxs-lookup"><span data-stu-id="95919-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="95919-106">Teie monitorid vilgub hetkega ja tulevad mõne sekundi pärast tagasi.</span><span class="sxs-lookup"><span data-stu-id="95919-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="95919-107">**Kuvari riistvara tõrkeotsing:**</span><span class="sxs-lookup"><span data-stu-id="95919-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="95919-108">Eemaldage kaabel, ühendades arvuti kuvariga, ja ühendage see uuesti.</span><span class="sxs-lookup"><span data-stu-id="95919-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="95919-109">Eemaldage ARVUTIST kõik mittevajalikud seadmed (nt adapterid või dokid).</span><span class="sxs-lookup"><span data-stu-id="95919-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="95919-110">**Kui olete hiljuti installinud värskenduse arvutisse, saate pöörata tagasi ekraani draiver:**</span><span class="sxs-lookup"><span data-stu-id="95919-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="95919-111">Valige **Start**, tippige **Seadmehaldur**ja valige tulemite hulgast **Seadmehaldur** .</span><span class="sxs-lookup"><span data-stu-id="95919-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="95919-112">Laiendage **Kuva adapterid** jaotis, paremklõpsake oma kuvaadapteri, ANDS valige **Atribuudid**.</span><span class="sxs-lookup"><span data-stu-id="95919-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="95919-113">Navigeerige vahekaardil **draiver** ja valige **draiveri tagasipööramise**nupp.</span><span class="sxs-lookup"><span data-stu-id="95919-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="95919-114">Märkused: kui see ei ole saadaval või on tuhmunud, valige **ei** alates alltoodud suvanditest järgmisele sammuks liikumiseks.</span><span class="sxs-lookup"><span data-stu-id="95919-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="95919-115">Enne muudatuste jõustumist peate võib-olla arvuti taaskäivitama.</span><span class="sxs-lookup"><span data-stu-id="95919-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="95919-116">**Desinstallige ja installige Kuva draiver uuesti:**</span><span class="sxs-lookup"><span data-stu-id="95919-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="95919-117">Valige **Start**, tippige **Seadmehaldur**ja valige tulemite hulgast **Seadmehaldur** .</span><span class="sxs-lookup"><span data-stu-id="95919-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="95919-118">Laiendage **Kuva adapterid** jaotis, paremklõpsake oma kuvaadapteri, ANDS valige **Uninstall seade**.</span><span class="sxs-lookup"><span data-stu-id="95919-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="95919-119">Valige **selle seadme draiveritarkvara kustutamise** kõrval olev ruut ja valige **Uninstall**.</span><span class="sxs-lookup"><span data-stu-id="95919-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="95919-120">Märkus: teil võidakse paluda oma arvuti selles etapis taaskäivitada.</span><span class="sxs-lookup"><span data-stu-id="95919-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="95919-121">Enne taaskäivitumist Kirjutage kindlasti ülejäänud juhised üles.</span><span class="sxs-lookup"><span data-stu-id="95919-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="95919-122">Avage Seadmehaldur uuesti.</span><span class="sxs-lookup"><span data-stu-id="95919-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="95919-123">Laiendage jaotist **Kuva adapterid** , paremklõpsake kuvaadapteri ja valige **Värskenda draiverit**.</span><span class="sxs-lookup"><span data-stu-id="95919-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="95919-124">Valige **draiveritarkvara värskendamiseks Automaatne otsing** ja järgige installijuhiseid.</span><span class="sxs-lookup"><span data-stu-id="95919-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>