---
title: Piirata juurdepääsu SharePointi või OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b6be074ed5f7e83f8196ca3fe90252673896569f
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29466387"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="55073-102">Piirata juurdepääsu SharePointi või OneDrive</span><span class="sxs-lookup"><span data-stu-id="55073-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="55073-p101">SharePointis või OneDrive, piirate üksuste failid, kaustad ja nimekirjad poolt juurdepääsu andmist ainult rühmadele ja üksikisikutele juurdepääsu teistele. Vaikimisi SharePointi õigused päritakse suurem üles hierarhia. Nii faili pärib oma õigused kausta, mis pärib oma õigused teegis, mis pärib oma õigused saidi.</span><span class="sxs-lookup"><span data-stu-id="55073-p101">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access. By default, permissions in SharePoint are inherited from higher up in the hierarchy. So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="55073-p102">Saate jagada on kõrgem (näiteks jagades kogu saidi) ja seejärel pärilust, kui te ei soovi kõiki üksusi kohapeal. Aga me ei soovita seda kuna tagab säilitada õigused keerukaid ja segase tulevikus. Siin on, mida võiks teha selle asemel:</span><span class="sxs-lookup"><span data-stu-id="55073-p102">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site. However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future. Here's what you could do instead:</span></span>
  
- <span data-ttu-id="55073-109">Kui näiteks soovite jagada välja arvatud see üks fail kausta sisu, selle faili teisaldada uude asukohta, mis ei ole jagatud.</span><span class="sxs-lookup"><span data-stu-id="55073-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="55073-110">Kui teil on kaks alamkaustad kausta ja jagada üks alamkausta A ja B rühma ja üksnes A rühma juurdepääsu teise alamkausta, jagada emakausta A rühma ja lisada B-grupi esimese alamkausta.</span><span class="sxs-lookup"><span data-stu-id="55073-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="55073-111">Faili või kausta ühiskasutuse peatamine</span><span class="sxs-lookup"><span data-stu-id="55073-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

