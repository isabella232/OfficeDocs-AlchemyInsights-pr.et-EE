---
title: Piirata juurdepääsu SharePointi või OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551447"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="0dba2-102">Piirata juurdepääsu SharePointi või OneDrive</span><span class="sxs-lookup"><span data-stu-id="0dba2-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="0dba2-103">SharePointis või OneDrive, piirate üksuste failid, kaustad ja nimekirjad poolt juurdepääsu andmist ainult rühmadele ja üksikisikutele juurdepääsu teistele.</span><span class="sxs-lookup"><span data-stu-id="0dba2-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="0dba2-104">Vaikimisi SharePointi õigused päritakse suurem üles hierarhia.</span><span class="sxs-lookup"><span data-stu-id="0dba2-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="0dba2-105">Nii faili pärib oma õigused kausta, mis pärib oma õigused teegis, mis pärib oma õigused saidi.</span><span class="sxs-lookup"><span data-stu-id="0dba2-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="0dba2-106">Saate jagada on kõrgem (näiteks jagades kogu saidi) ja seejärel pärilust, kui te ei soovi kõiki üksusi kohapeal.</span><span class="sxs-lookup"><span data-stu-id="0dba2-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="0dba2-107">Aga me ei soovita seda kuna tagab säilitada õigused keerukaid ja segase tulevikus.</span><span class="sxs-lookup"><span data-stu-id="0dba2-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="0dba2-108">Siin on, mida võiks teha selle asemel:</span><span class="sxs-lookup"><span data-stu-id="0dba2-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="0dba2-109">Kui näiteks soovite jagada välja arvatud see üks fail kausta sisu, selle faili teisaldada uude asukohta, mis ei ole jagatud.</span><span class="sxs-lookup"><span data-stu-id="0dba2-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="0dba2-110">Kui teil on kaks alamkaustad kausta ja jagada üks alamkausta A ja B rühma ja üksnes A rühma juurdepääsu teise alamkausta, jagada emakausta A rühma ja lisada B-grupi esimese alamkausta.</span><span class="sxs-lookup"><span data-stu-id="0dba2-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="0dba2-111">Faili või kausta ühiskasutuse peatamine</span><span class="sxs-lookup"><span data-stu-id="0dba2-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

