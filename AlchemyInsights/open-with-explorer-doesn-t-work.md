---
title: Ava Explorer ei tööta
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: b55fc7bd5670e655334ef7be368b245c8899633a
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28284971"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="ab8e3-102">Ava Explorer ei tööta</span><span class="sxs-lookup"><span data-stu-id="ab8e3-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="ab8e3-p101">Kui **Ava Explorer** või **File Exploreris** ei tööta veenduge, WebClient teenuse seatakse **töötab** , järgmisi juhiseid. Näiteks võib kuluda kaua aega OneDrive'i või SharePointi teegi avamiseks, kui teenus on peatatud.</span><span class="sxs-lookup"><span data-stu-id="ab8e3-p101">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below. For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="ab8e3-105">Otsinguväljale Windows käivitada, tüüp valige Käivita töölauarakendust, tüüp services.msc ja seejärel valige **Sisesta**.</span><span class="sxs-lookup"><span data-stu-id="ab8e3-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="ab8e3-p102">Kerige WebClient teenuse ja vaadake veerust **olek** . Kui WebClient teenuse olek ei **tööta**, topeltklõpsake teenust, klõpsake nuppu **Start**ja klõpsake **OK**. Lubage teenus, vajadusel valige **käsitsi** või **automaatse** **käivituse** tüüp.</span><span class="sxs-lookup"><span data-stu-id="ab8e3-p102">Scroll down to the WebClient service and check the **Status** column. If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**. Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="ab8e3-p103">File Exploreri avamine tõrkeotsingu, vt [Exploreris avatud](https://go.microsoft.com/fwlink/?linkid=871665). Uurida sünkroonimise parem alternatiiv: [uue OneDrive'i sünkroonimisrakenduse sünkroonimine SharePointi faile](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="ab8e3-p103">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

