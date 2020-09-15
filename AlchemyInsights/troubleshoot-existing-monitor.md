---
title: Olemasoleva kuvari tõrkeotsing
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
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690707"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="a287f-102">Olemasoleva kuvari tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="a287f-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="a287f-103">Proovige järgmisi lahendusi kuvari tõrkeotsinguks.</span><span class="sxs-lookup"><span data-stu-id="a287f-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="a287f-104">**Kuvari kuvari värskendamine.**</span><span class="sxs-lookup"><span data-stu-id="a287f-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="a287f-105">Vajutage samal ajal järgmisi klahve: Windowsi klahv + CTRL + SHIFT + B. See värskendab suhtlemist teie graafika draiveriga.</span><span class="sxs-lookup"><span data-stu-id="a287f-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="a287f-106">Teie kuvarid vilgub hetkega ja need tulevad mõne sekundi pärast tagasi.</span><span class="sxs-lookup"><span data-stu-id="a287f-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="a287f-107">**Kuvari riistvara tõrkeotsing.**</span><span class="sxs-lookup"><span data-stu-id="a287f-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="a287f-108">Lahutage kaabel, ühendades arvuti kuvariga, ja ühendage see uuesti.</span><span class="sxs-lookup"><span data-stu-id="a287f-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="a287f-109">Lahutage ARVUTIST kõik ebaolulised seadmed (nt adapterid või dokid).</span><span class="sxs-lookup"><span data-stu-id="a287f-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="a287f-110">**Kui installisite hiljuti oma ARVUTISSE värskenduse, saate oma kuvari draiveri tagasi pöörata.**</span><span class="sxs-lookup"><span data-stu-id="a287f-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="a287f-111">Valige **Start**, tippige **Seadmehaldur**ja valige tulemitest **Seadmehaldur** .</span><span class="sxs-lookup"><span data-stu-id="a287f-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="a287f-112">Laiendage jaotist **kuvari adapterid** , paremklõpsake oma kuvari adapterit, valige ANDS **Atribuudid**.</span><span class="sxs-lookup"><span data-stu-id="a287f-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="a287f-113">Liikuge menüüsse **draiver** ja valige **draiveri tagasipööramine**.</span><span class="sxs-lookup"><span data-stu-id="a287f-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="a287f-114">Märkus: kui see pole saadaval või on tuhm **, valige järgmise** juhise juurde liikumiseks allpool olevatest valikutest.</span><span class="sxs-lookup"><span data-stu-id="a287f-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="a287f-115">Enne nende muudatuste jõustumist peate võib-olla arvuti taaskäivitama.</span><span class="sxs-lookup"><span data-stu-id="a287f-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="a287f-116">**Draiveri desinstallimine ja uuesti installimine.**</span><span class="sxs-lookup"><span data-stu-id="a287f-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="a287f-117">Valige **Start**, tippige **Seadmehaldur**ja valige tulemitest **Seadmehaldur** .</span><span class="sxs-lookup"><span data-stu-id="a287f-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="a287f-118">Laiendage jaotist **kuvari adapterid** , paremklõpsake kuvari adapterit, ANDS valige **Uninstall Device (Desinstalli seade**).</span><span class="sxs-lookup"><span data-stu-id="a287f-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="a287f-119">Valige **selle seadme draiveri tarkvara kustutamise** kõrval olev väli ja valige **Uninstall (Desinstalli**).</span><span class="sxs-lookup"><span data-stu-id="a287f-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="a287f-120">Märkus: teil võidakse paluda arvuti taaskäivitada selles etapis.</span><span class="sxs-lookup"><span data-stu-id="a287f-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="a287f-121">Enne taaskäivitamist veenduge, et enne uuesti kirjutamist kuvataks ülejäänud juhised.</span><span class="sxs-lookup"><span data-stu-id="a287f-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="a287f-122">Avage Device Manager uuesti.</span><span class="sxs-lookup"><span data-stu-id="a287f-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="a287f-123">Laiendage jaotist **kuvari adapterid** , paremklõpsake oma kuvari adapterit ja valige **draiveri värskendamine**.</span><span class="sxs-lookup"><span data-stu-id="a287f-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="a287f-124">**Draiveri tarkvara värskendamiseks valige Otsi automaatselt** ja järgige installijuhiseid.</span><span class="sxs-lookup"><span data-stu-id="a287f-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>