---
title: Olemasoleva kuvari tõrkeotsing
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
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824575"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="5b36e-102">Olemasoleva kuvari tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="5b36e-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="5b36e-103">Proovige neid lahendusi kuvari tõrkeotsinguks.</span><span class="sxs-lookup"><span data-stu-id="5b36e-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="5b36e-104">**Kuvari kuva värskendamine**</span><span class="sxs-lookup"><span data-stu-id="5b36e-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="5b36e-105">Vajutage korraga järgmisi klahve: Windowsi klahv + Ctrl + Shift + B. See värskendab suhtlust graafikadraiveriga.</span><span class="sxs-lookup"><span data-stu-id="5b36e-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="5b36e-106">Teie kuvarid vilguvad hetkega ja tulevad mõne sekundi pärast tagasi.</span><span class="sxs-lookup"><span data-stu-id="5b36e-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="5b36e-107">**Kuvari riistvara tõrkeotsing.**</span><span class="sxs-lookup"><span data-stu-id="5b36e-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="5b36e-108">Ühendage arvuti kuvariga ühendav kaabel ja ühendage see uuesti sisse.</span><span class="sxs-lookup"><span data-stu-id="5b36e-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="5b36e-109">Ühendage arvutist lahti kõik mitte hädavajalikud seadmed (nt adapterid või dokid).</span><span class="sxs-lookup"><span data-stu-id="5b36e-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="5b36e-110">**Kui olete hiljuti arvutisse värskenduse installinud, saate kuvadraiveri tagasi pöörata.**</span><span class="sxs-lookup"><span data-stu-id="5b36e-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="5b36e-111">Valige **Start**, tippige **seadmehaldur** ja valige **tulemitest** Seadmehaldur.</span><span class="sxs-lookup"><span data-stu-id="5b36e-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="5b36e-112">Laiendage **jaotist Kuvaadapterid,** paremklõpsake kuvaadapterit ja valige **Atribuudid**.</span><span class="sxs-lookup"><span data-stu-id="5b36e-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="5b36e-113">Liikuge vahekaardile **Draiver** ja valige **Draiveri tagasipööramine**.</span><span class="sxs-lookup"><span data-stu-id="5b36e-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="5b36e-114">Märkus. Kui see pole saadaval või on  tuhm, valige järgmise juhise juurde liikumiseks allolevatest suvanditest Ei.</span><span class="sxs-lookup"><span data-stu-id="5b36e-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="5b36e-115">Võimalik, et peate enne nende muudatuste jõustumist arvuti taaskäivitama.</span><span class="sxs-lookup"><span data-stu-id="5b36e-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="5b36e-116">**Desinstallige kuvadraiver ja installige see uuesti.**</span><span class="sxs-lookup"><span data-stu-id="5b36e-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="5b36e-117">Valige **Start**, tippige **seadmehaldur** ja valige **tulemitest** Seadmehaldur.</span><span class="sxs-lookup"><span data-stu-id="5b36e-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="5b36e-118">Laiendage **jaotist Kuvaadapterid,** paremklõpsake kuvaadapterit ja valige **Desinstalli seade.**</span><span class="sxs-lookup"><span data-stu-id="5b36e-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="5b36e-119">Märkige ruut Kustuta selle **seadme draiveritarkvara ja valige** **Desinstalli**.</span><span class="sxs-lookup"><span data-stu-id="5b36e-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="5b36e-120">Märkus. Teil võidakse paluda oma arvuti selles etapis taaskäivitada.</span><span class="sxs-lookup"><span data-stu-id="5b36e-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="5b36e-121">Enne taaskäivitamist kirjutage ülejäänud juhised kindlasti üles.</span><span class="sxs-lookup"><span data-stu-id="5b36e-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="5b36e-122">Avage uuesti Seadmehaldur.</span><span class="sxs-lookup"><span data-stu-id="5b36e-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="5b36e-123">Laiendage **jaotist Kuvaadapterid,** paremklõpsake kuvaadapterit ja valige Värskenda **draiverit.**</span><span class="sxs-lookup"><span data-stu-id="5b36e-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="5b36e-124">Valige **Otsi draiveri tarkvara värskendamiseks automaatselt** ja järgige installijuhiseid.</span><span class="sxs-lookup"><span data-stu-id="5b36e-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>