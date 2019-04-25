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
ms.openlocfilehash: 73d33e50449345c312abdd39afcc36e0c95fd1c4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32419866"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="ccb5a-102">Ava Explorer ei tööta</span><span class="sxs-lookup"><span data-stu-id="ccb5a-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="ccb5a-103">Kui **Ava Explorer** või **File Exploreris** ei tööta veenduge, WebClient teenuse seatakse **töötab** , järgmisi juhiseid.</span><span class="sxs-lookup"><span data-stu-id="ccb5a-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="ccb5a-104">Näiteks võib kuluda kaua aega OneDrive'i või SharePointi teegi avamiseks, kui teenus on peatatud.</span><span class="sxs-lookup"><span data-stu-id="ccb5a-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="ccb5a-105">Otsinguväljale Windows käivitada, tüüp valige Käivita töölauarakendust, tüüp services.msc ja seejärel valige **Sisesta**.</span><span class="sxs-lookup"><span data-stu-id="ccb5a-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="ccb5a-106">Kerige WebClient teenuse ja vaadake veerust **olek** .</span><span class="sxs-lookup"><span data-stu-id="ccb5a-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="ccb5a-107">Kui WebClient teenuse olek ei **tööta**, topeltklõpsake teenust, klõpsake nuppu **Start**ja klõpsake **OK**.</span><span class="sxs-lookup"><span data-stu-id="ccb5a-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="ccb5a-108">Lubage teenus, vajadusel valige **käsitsi** või **automaatse** **käivituse** tüüp.</span><span class="sxs-lookup"><span data-stu-id="ccb5a-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="ccb5a-109">File Exploreri avamine tõrkeotsingu, vt [Exploreris avatud](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="ccb5a-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="ccb5a-110">Uurida sünkroonimise parem alternatiiv: [uue OneDrive'i sünkroonimisrakenduse sünkroonimine SharePointi faile](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="ccb5a-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

