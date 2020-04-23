---
title: Profiili sünkroonimine
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768109"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="87937-102">Millal muudab profiil SharePointi kasutajaprofiili rakenduse sünkroonimist?</span><span class="sxs-lookup"><span data-stu-id="87937-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="87937-103">SharePoint Online kasutab Active Directory importimine ajastitöö (AD import) kasutajate ja rühmade importimiseks kasutajaprofiili rakendusse.</span><span class="sxs-lookup"><span data-stu-id="87937-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="87937-104">AD impordi sünkroonib muudatused SharePoint Online ' i Kataloogipoest kasutajaprofiili rakendus.</span><span class="sxs-lookup"><span data-stu-id="87937-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="87937-105">Neid muudatusi töödeldakse partiidena.</span><span class="sxs-lookup"><span data-stu-id="87937-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="87937-106">Ajastitöö töötab seni, kuni muudatused sünkroonitakse.</span><span class="sxs-lookup"><span data-stu-id="87937-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="87937-107">Töö käivitamiseks kuluv aeg sõltub protsessi muutuste arvust.</span><span class="sxs-lookup"><span data-stu-id="87937-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="87937-108">Suur hulk muudatusi võtab kauem aega.</span><span class="sxs-lookup"><span data-stu-id="87937-108">A large number of changes takes longer.</span></span> <span data-ttu-id="87937-109">Teenusetaseme leping (SLA) teatab, et kasutaja SharePoint Online ' i kataloogi muutmine kajastub kasutajaprofiili rakenduse 24 tunni jooksul.</span><span class="sxs-lookup"><span data-stu-id="87937-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="87937-110">Rohkem infot Kasutajaprofiili sünkroonimise kohta SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="87937-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

