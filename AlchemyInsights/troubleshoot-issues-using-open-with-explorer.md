---
title: Tõrkeotsingu funktsiooniga Ava Exploreris
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 03bb3ad01a716390ec50845b29ddf6cc81a83116
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/22/2019
ms.locfileid: "30759290"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="d3537-102">Lahendamiseks Ava Explorer</span><span class="sxs-lookup"><span data-stu-id="d3537-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="d3537-103">Levinud probleemide ja seejärel käsku **Ava Explorer** OneDrive'i või SharePointi dokumenditeegi avamine:</span><span class="sxs-lookup"><span data-stu-id="d3537-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="d3537-104">Kasutage Internet Explorer 10 või Internet Exploreri 11.</span><span class="sxs-lookup"><span data-stu-id="d3537-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="d3537-105">**Ava Explorer** ei ühildu Microsoft Edge, Google Chrome, Firefox ja teised.</span><span class="sxs-lookup"><span data-stu-id="d3537-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="d3537-106">**Ava Explorer** on keelatud kõik brauserid, välja arvatud Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="d3537-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="d3537-107">**Ava Explorer** pole saadaval kaasaegne kogemus SharePointi teekides.</span><span class="sxs-lookup"><span data-stu-id="d3537-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="d3537-108">Kasutage **File Exploreris** .</span><span class="sxs-lookup"><span data-stu-id="d3537-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="d3537-109">Valige **vaates Valikud** \> **File Exploreris**.</span><span class="sxs-lookup"><span data-stu-id="d3537-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="d3537-110">File Exploreris ei ühildu Microsoft Edge, Google Chrome, Firefox ja teised.</span><span class="sxs-lookup"><span data-stu-id="d3537-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="d3537-111">**File Exploreris** saadaval ainult Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="d3537-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="d3537-112">Veenduge, et WebClient teenus töötab.</span><span class="sxs-lookup"><span data-stu-id="d3537-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="d3537-113">Otsinguväljale Windows tippige Käivita, valige Käivita töölauarakendust, tüüp services.msc ja seejärel vajutage Enter.</span><span class="sxs-lookup"><span data-stu-id="d3537-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="d3537-114">Kerige WebClient teenus ja veenduge, et selle **olek** veerus kuvatakse "Käivitamine."</span><span class="sxs-lookup"><span data-stu-id="d3537-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="d3537-115">Kui seda pole, topeltklõpsake teenuse, klõpsake **Start**ja seejärel klõpsake nuppu **OK**.</span><span class="sxs-lookup"><span data-stu-id="d3537-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="d3537-116">(Võimalik, et peate esmalt lubama teenuse valides kas **käsitsi** või **automaatse** **käivituse** tüüp.)</span><span class="sxs-lookup"><span data-stu-id="d3537-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="d3537-117">File Exploreris Raamatukogu avamine on mugav, kui soovite kopeerida või teisaldada mitu faile ja kaustu, kui, kuid kui soovite regulaarselt töötada raamatukogus, soovitame sünkroonimist.</span><span class="sxs-lookup"><span data-stu-id="d3537-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="d3537-118">File Exploreri avamine tõrkeotsingu, vt [Exploreris avatud](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="d3537-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="d3537-119">Sünkroonimise häälestamise kohta leiate teemast [uue OneDrive'i sünkroonimisrakenduse sünkroonimine SharePointi faile](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="d3537-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="d3537-120">Vaadake lisateavet artikli ["avatud koos Explorer" käsu tõrkeotsingu SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) .</span><span class="sxs-lookup"><span data-stu-id="d3537-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  

