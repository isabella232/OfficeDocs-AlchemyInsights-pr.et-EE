---
title: Tõrkeotsing probleemidele, kasutades Open Exploreriga
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
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742729"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="67739-102">Ava Exploreriga seotud probleemide lahendamine</span><span class="sxs-lookup"><span data-stu-id="67739-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="67739-103">Lahendada levinud probleemid avamisel dokumenditeeki rakenduses SharePoint või OneDrive **Open Explorer** käsu abil:</span><span class="sxs-lookup"><span data-stu-id="67739-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="67739-104">Kasutage Internet Explorer 10 või Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="67739-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="67739-105">**Exploreriga avamine** ei ühildu Microsoft Edge ' i, Google Chrome ' i, Firefoxi ja teistega.</span><span class="sxs-lookup"><span data-stu-id="67739-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="67739-106">**Avatud Explorer** on keelatud kõigis brauserites peale Internet Exploreri.</span><span class="sxs-lookup"><span data-stu-id="67739-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="67739-107">**Avatud Explorer** ei ole saadaval kaasaegne kogemus SharePointi teegid.</span><span class="sxs-lookup"><span data-stu-id="67739-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="67739-108">Kasutage **Vaade File Exploreris** .</span><span class="sxs-lookup"><span data-stu-id="67739-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="67739-109">Valige Kuva **Suvandid** \> **Vaade File Exploreris**.</span><span class="sxs-lookup"><span data-stu-id="67739-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="67739-110">Vaade File Exploreris ei ühildu Microsoft Edge ' i, Google Chrome ' i, Firefoxi ja teistega.</span><span class="sxs-lookup"><span data-stu-id="67739-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="67739-111">**Vaade File Exploreris** saadaval ainult Internet Exploreris.</span><span class="sxs-lookup"><span data-stu-id="67739-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="67739-112">Veenduge, et WebClient teenus töötab.</span><span class="sxs-lookup"><span data-stu-id="67739-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="67739-113">Windowsi otsinguväljale tippige Run, valige Käivita töölauarakendus, tippige Services. mscja vajutage sisestusklahvi ENTER.</span><span class="sxs-lookup"><span data-stu-id="67739-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="67739-114">Kerige WebClient teenuse ja veenduge, et **olek** veerus kuvatakse "töötab."</span><span class="sxs-lookup"><span data-stu-id="67739-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="67739-115">Kui ei, topeltklõpsake teenust, klõpsake nuppu **Start**ja seejärel klõpsake nuppu **OK**.</span><span class="sxs-lookup"><span data-stu-id="67739-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="67739-116">(Võib-olla peate teenuse esmalt lubama, valides **käivitustüübi** väljal **käsitsi** või **automaatselt** .)</span><span class="sxs-lookup"><span data-stu-id="67739-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="67739-117">Teegi avamine File Exploreris on mugav, kui teil on vaja mitu faili ja kausta korraga kopeerida või teisaldada, kuid kui soovite teegis regulaarselt töötada, soovitame seda sünkroonida.</span><span class="sxs-lookup"><span data-stu-id="67739-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="67739-118">File Exploreris avamise probleemide tõrkeotsinguks vaadake [avatud Exploreris](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="67739-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="67739-119">Sünkroonimise seadistamise kohta teabe saamiseks vaadake [SharePointi failide sünkroonimine uue OneDrive ' i sünkroonimiskliendiga](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="67739-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="67739-120">Lugege artiklit, [Kuidas kasutada käsku "Open with Explorer" tõrkeotsing SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) ' i probleemide kohta lisateabe saamiseks.</span><span class="sxs-lookup"><span data-stu-id="67739-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

