---
title: SharePointi või OneDrive ' i juurdepääsu piiramine
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: ed8e97b20c96a7b46995c969074cc4cef3a787d9
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715880"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="83a2d-102">SharePointi või OneDrive ' i juurdepääsu piiramine</span><span class="sxs-lookup"><span data-stu-id="83a2d-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="83a2d-103">SharePointis ja OneDrive ' is saate piirata juurdepääsu sellistele üksustele nagu failid, kaustad ja loendid, andes juurdepääsu ainult rühmadele või üksikisikutele, kellele soovite juurdepääsu.</span><span class="sxs-lookup"><span data-stu-id="83a2d-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="83a2d-104">Vaikimisi on SharePointi õigused päritud hierarhias kõrgemale.</span><span class="sxs-lookup"><span data-stu-id="83a2d-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="83a2d-105">Seega päriab fail oma õigused kaustast, mis päriab oma load teegist, mis päriab oma õigused saidilt.</span><span class="sxs-lookup"><span data-stu-id="83a2d-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="83a2d-106">Saate jagada kõrgema taseme (nt jagades kogu saidi) ja seejärel murda pärand, kui te ei soovi jagada kõik üksused saidil.</span><span class="sxs-lookup"><span data-stu-id="83a2d-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="83a2d-107">Kuid me ei soovita seda, sest see muudab õiguste säilitamise keerulisemaks ja segadust tulevikus.</span><span class="sxs-lookup"><span data-stu-id="83a2d-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="83a2d-108">Selle asemel saate teha järgmist.</span><span class="sxs-lookup"><span data-stu-id="83a2d-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="83a2d-109">Kui näiteks soovite ühiskasutada kogu kausta sisu, välja arvatud üks fail, teisaldage see fail uude asukohta, mida ei jagata.</span><span class="sxs-lookup"><span data-stu-id="83a2d-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="83a2d-110">Kui teil on kaustas kaks alamkausta ja soovite jagada rühmi A ja B ühe alamkaustaga ja lubada ainult rühma A juurdepääsu teisele alamkaustale, Jagage emakausta A rühmaga ja lisage rühm B esimesele alamkaustale.</span><span class="sxs-lookup"><span data-stu-id="83a2d-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="83a2d-111">Faili või kausta ühiskasutuse peatamine</span><span class="sxs-lookup"><span data-stu-id="83a2d-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

