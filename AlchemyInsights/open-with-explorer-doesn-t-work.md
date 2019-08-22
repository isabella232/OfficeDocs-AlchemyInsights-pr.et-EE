---
title: Ava Explorer ei tööta
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 7680766b53bd5e85789375d3f9e9ab635780ec6c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538463"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="b39e5-102">Ava Explorer ei tööta</span><span class="sxs-lookup"><span data-stu-id="b39e5-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="b39e5-103">Kui **Ava Explorer** või **File Exploreris** ei tööta veenduge, WebClient teenuse seatakse **töötab** , järgmisi juhiseid.</span><span class="sxs-lookup"><span data-stu-id="b39e5-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="b39e5-104">Näiteks võib kuluda kaua aega OneDrive'i või SharePointi teegi avamiseks, kui teenus on peatatud.</span><span class="sxs-lookup"><span data-stu-id="b39e5-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="b39e5-105">Otsinguväljale Windows käivitada, tüüp valige Käivita töölauarakendust, tüüp services.msc ja seejärel valige **Sisesta**.</span><span class="sxs-lookup"><span data-stu-id="b39e5-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="b39e5-106">Kerige WebClient teenuse ja vaadake veerust **olek** .</span><span class="sxs-lookup"><span data-stu-id="b39e5-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="b39e5-107">Kui WebClient teenuse olek ei **tööta**, topeltklõpsake teenust, klõpsake nuppu **Start**ja klõpsake **OK**.</span><span class="sxs-lookup"><span data-stu-id="b39e5-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="b39e5-108">Lubage teenus, vajadusel valige **käsitsi** või **automaatse** **käivituse** tüüp.</span><span class="sxs-lookup"><span data-stu-id="b39e5-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="b39e5-109">File Exploreri avamine tõrkeotsingu, vt [Exploreris avatud](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="b39e5-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="b39e5-110">Uurida sünkroonimise parem alternatiiv: [uue OneDrive'i sünkroonimisrakenduse sünkroonimine SharePointi faile](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="b39e5-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

