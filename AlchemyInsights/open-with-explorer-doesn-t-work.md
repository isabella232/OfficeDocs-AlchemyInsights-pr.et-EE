---
title: Avatud Exploreriga ei tööta
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713030"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="4d3c9-102">Avatud Exploreriga ei tööta</span><span class="sxs-lookup"><span data-stu-id="4d3c9-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="4d3c9-103">Kui **avatud Explorer** või **Vaade File Explorer** ei tööta veenduge, et WebClient teenus on seatud **töötama** , järgides alltoodud juhiseid.</span><span class="sxs-lookup"><span data-stu-id="4d3c9-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="4d3c9-104">Näiteks võib kuluda kaua aega, et avada SharePointi või OneDrive Raamatukogu, kui teenus ei tööta.</span><span class="sxs-lookup"><span data-stu-id="4d3c9-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="4d3c9-105">Tippige Windowsi otsinguväljale käsk Käivita, valige Käivita töölauarakendus, tippige Services. mscja seejärel valige käsk **Sisesta**.</span><span class="sxs-lookup"><span data-stu-id="4d3c9-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="4d3c9-106">Kerige WebClient teenuse ja kontrollige **oleku** veerg.</span><span class="sxs-lookup"><span data-stu-id="4d3c9-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="4d3c9-107">Kui WebClient teenuse olek ei **tööta**, topeltklõpsake teenust, klõpsake nuppu **Start**ja seejärel klõpsake nuppu **OK**.</span><span class="sxs-lookup"><span data-stu-id="4d3c9-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="4d3c9-108">Vajaduse korral lubage teenus, valides **käivitustüübi** väljal kas **käsitsi** või **automaatse** .</span><span class="sxs-lookup"><span data-stu-id="4d3c9-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="4d3c9-109">File Exploreris avamise probleemide tõrkeotsinguks vaadake [avatud Exploreris](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="4d3c9-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="4d3c9-110">Avastage sünkroonimine parema võimalusena: [SharePointi failide sünkroonimine uue OneDrive ' i sünkroonimiskliendiga](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="4d3c9-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

