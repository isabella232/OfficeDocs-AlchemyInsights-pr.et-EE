---
title: Käsu Ava Exploreris probleemide tõrkeotsing SharePoint Online’is
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 8/7/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 21a0c193b752342d47189dda73d171249153f7fc
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050809"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="25bf1-102">Käsu Ava Exploreris probleemide tõrkeotsing SharePoint Online’is</span><span class="sxs-lookup"><span data-stu-id="25bf1-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="25bf1-103">Käsk Ava Exploreris avab Windows Exploreri kohaliku eksemplari, mis kuvab SharePointi saiti majutava serveri kausta struktuuri.</span><span class="sxs-lookup"><span data-stu-id="25bf1-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="25bf1-104">Seetõttu soovitame [sünkroonida SharePointi failid uue OneDrive’i sünkroonimisrakendusega](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a>, mis pakub [nõudefaile](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e), kuna see võimaldab failidele kohalikku juurdepääsu ja pakub parimat jõudlust.</span><span class="sxs-lookup"><span data-stu-id="25bf1-104">This being said, we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="25bf1-105">Kui otsustasite uue sünkroonimisrakenduse asemel kasutada Exploreri vaadet, siis veenduge, et järgiksite järgmistes artiklites toodud juhendeid ja häid tavasid:</span><span class="sxs-lookup"><span data-stu-id="25bf1-105">If you chose to use Explorer view instead of using the new OneDrive sync client, make sure you follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="25bf1-106">SharePoint Online’i probleemide tõrkeotsinguks käsu Ava Exploreris kasutamine</span><span class="sxs-lookup"><span data-stu-id="25bf1-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)

- [<span data-ttu-id="25bf1-107">Käsu Ava Exploreris abil teegifailide kopeerimine või teisaldamine</span><span class="sxs-lookup"><span data-stu-id="25bf1-107">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

> [!Note]  
> <span data-ttu-id="25bf1-108">Uues teegi versioonis nuppu **Ava Exploreris** ei ole.</span><span class="sxs-lookup"><span data-stu-id="25bf1-108">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="25bf1-109">Klõpsake üleval paremal rippmenüüd **Vaade** (rippmenüü nimi muutub olenevalt teie praegusest vaatest) ja seejärel valige **Vaade File Exploreris**.</span><span class="sxs-lookup"><span data-stu-id="25bf1-109">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>
>
 ><span data-ttu-id="25bf1-110">SharePointi käsk Ava Exploreris kasutab ActiveX-juhtelemente, mistõttu seda toetatakse ainult Internet Exploreri versioonis 10 või 11.</span><span class="sxs-lookup"><span data-stu-id="25bf1-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="25bf1-111">Käsk Ava Exploreris ei tööta Windowsis Microsoft Edge’i, Google Chrome’i, Mozilla Firefoxi ega Maci platvormiga.</span><span class="sxs-lookup"><span data-stu-id="25bf1-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="25bf1-112">Seepärast võib suvand Exploreri vaade olla kuvatud tuhmina.</span><span class="sxs-lookup"><span data-stu-id="25bf1-112">Due to this reason, the Explorer View option may be grayed out.</span></span>
>
> - <span data-ttu-id="25bf1-113">[Miks pole SharePointi lindi nupud kättesaadavad või on tuhmid](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca)?</span><span class="sxs-lookup"><span data-stu-id="25bf1-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

