---
title: Avamine Exploreris ei tööta
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694452"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="32c50-102">Avamine Exploreris ei tööta</span><span class="sxs-lookup"><span data-stu-id="32c50-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="32c50-103">Kui **Open with Explorer** või **Vaade failis Explorer** ei tööta, siis veenduge, et webclienti teenus oleks seatud toimima **, järgides** allolevaid juhiseid.</span><span class="sxs-lookup"><span data-stu-id="32c50-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="32c50-104">Näiteks võib kuluda pikk aeg, et avada SharePointi või OneDrive ' i teek, kui teenus ei tööta.</span><span class="sxs-lookup"><span data-stu-id="32c50-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="32c50-105">Tippige Windowsi otsinguväljale tekst Käivita, valige Käivita töölauarakendus, tippige tekst Services. msc ja seejärel valige **sisestusklahv (ENTER)**.</span><span class="sxs-lookup"><span data-stu-id="32c50-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="32c50-106">Liikuge kerides Webclienti teenuse juurde ja kontrollige veergu **olek** .</span><span class="sxs-lookup"><span data-stu-id="32c50-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="32c50-107">Kui Webclienti teenuse olek ei **tööta**, topeltklõpsake teenust, klõpsake nuppu **Start**ja seejärel nuppu **OK**.</span><span class="sxs-lookup"><span data-stu-id="32c50-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="32c50-108">Vajadusel teenuse lubamiseks valige väljal **Käivitustüüp** kas **käsitsi** või **Automaatne** .</span><span class="sxs-lookup"><span data-stu-id="32c50-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="32c50-109">Faili Exploreris avamisega seotud probleemide tõrkeotsingu kohta leiate teavet teemast [Ava Exploreris](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="32c50-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="32c50-110">Uurige sünkroonimist parema alternatiivina: [SharePointi failide sünkroonimine uue OneDrive ' i sünkroonimise klientrakendusega](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="32c50-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

