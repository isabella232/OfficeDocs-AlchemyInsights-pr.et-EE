---
title: Tõrkeotsing probleemidele avamisel Exploreri abil
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659054"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="f64c3-102">Exploreri avamisega seotud probleemide lahendamine</span><span class="sxs-lookup"><span data-stu-id="f64c3-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="f64c3-103">Levinud probleemide lahendamine dokumenditeegi avamisel SharePointis või OneDrive ' is käsu **Ava Exploreris** abil</span><span class="sxs-lookup"><span data-stu-id="f64c3-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="f64c3-104">Kasutage Internet Explorer 10 või Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="f64c3-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="f64c3-105">**Exploreri avamine** ei ühildu Microsoft Edge ' i, Google Chrome ' i, Firefoxi ja teiste kasutajatega.</span><span class="sxs-lookup"><span data-stu-id="f64c3-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="f64c3-106">**Exploreris avamine** on keelatud kõigis brauserites (v. a Internet Explorer).</span><span class="sxs-lookup"><span data-stu-id="f64c3-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="f64c3-107">**Rakendusega Explorer** pole saadaval SharePointi teekide moodsas versioonis.</span><span class="sxs-lookup"><span data-stu-id="f64c3-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="f64c3-108">Kasutage selle asemel **vaadet Explorer** .</span><span class="sxs-lookup"><span data-stu-id="f64c3-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="f64c3-109">Valige **Kuva suvandite** \> **Vaade failis Explorer**.</span><span class="sxs-lookup"><span data-stu-id="f64c3-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="f64c3-110">Vaade failis Explorer ei ühildu Microsoft Edge ' i, Google Chrome ' i, Firefoxi ja teiste kasutajatega.</span><span class="sxs-lookup"><span data-stu-id="f64c3-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="f64c3-111">**Kuvage failis Explorer** rakenduses Internet Explorer saadaval ainult.</span><span class="sxs-lookup"><span data-stu-id="f64c3-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="f64c3-112">Veenduge, et Webclienti teenus töötaks.</span><span class="sxs-lookup"><span data-stu-id="f64c3-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="f64c3-113">Tippige Windowsi otsinguväljale tekst Käivita, valige Käivita töölauarakendus, tippige tekst Services. msc ja seejärel vajutage sisestusklahvi (ENTER).</span><span class="sxs-lookup"><span data-stu-id="f64c3-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="f64c3-114">Liikuge kerides Webclienti teenuse juurde ja veenduge, et veerus **olek** kuvatakse tekst "töötab".</span><span class="sxs-lookup"><span data-stu-id="f64c3-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="f64c3-115">Kui seda ei juhtu, topeltklõpsake teenust, klõpsake nuppu **Start**ja seejärel nuppu **OK**.</span><span class="sxs-lookup"><span data-stu-id="f64c3-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="f64c3-116">(Võimalik, et peate esmalt lubama teenuse, valides väljale **Käivitustüüp** kas **käsitsi** või **automaatselt** .)</span><span class="sxs-lookup"><span data-stu-id="f64c3-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="f64c3-117">Teegi avamine rakenduses Explorer on mugav, kui peate mitu faili ja kausta korraga kopeerima või teisaldama, kuid kui soovite teegis regulaarselt töötada, soovitame seda sünkroonida.</span><span class="sxs-lookup"><span data-stu-id="f64c3-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="f64c3-118">Faili Exploreris avamisega seotud probleemide tõrkeotsingu kohta leiate teavet teemast [Ava Exploreris](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="f64c3-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="f64c3-119">Lisateavet sünkroonimise häälestamise kohta leiate teemast [SharePointi failide sünkroonimine uue OneDrive ' i sünkroonimise klientrakendusega](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="f64c3-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="f64c3-120">Lisateavet [SharePoint Online ' i probleemide tõrkeotsingu kohta leiate artiklist Kuidas kasutada käsku "Ava Explorer"](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) .</span><span class="sxs-lookup"><span data-stu-id="f64c3-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

