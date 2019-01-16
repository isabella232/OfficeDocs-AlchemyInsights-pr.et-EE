---
title: Profiilisünkroonimise
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a32cf9e623d1be7a2c85ef4951c6eb7f001b7db0
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28285521"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="8c521-102">Kuna minu profiili muudatused sünkroonida SharePointi kasutajaprofiili rakendusel?</span><span class="sxs-lookup"><span data-stu-id="8c521-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="8c521-103">SharePoint Online kasutab Active Directory importimine ajastitöö (AD Import) importimiseks kasutaja profiili rakenduse kasutajad ja rühmad.</span><span class="sxs-lookup"><span data-stu-id="8c521-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="8c521-p101">AD impordi sünkroonib muudatused SharePoint Online kataloogi poest kasutajaprofiili rakendusel. Need muutused jõustuvad partiina.</span><span class="sxs-lookup"><span data-stu-id="8c521-p101">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application. These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="8c521-106">Ajastitöö töötab kuni muudatused on sünkroonitud.</span><span class="sxs-lookup"><span data-stu-id="8c521-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="8c521-p102">Töö, mis käivitatakse kuluv aeg sõltub muutuste protsessi. Mitmeid muudatusi võtab kauem aega. Teenuse teenindustaseme lepingut (SLA) märgib, et SharePoint Online kataloogis kasutaja muutmine kajastub kasutajaprofiili rakendusel 24 tunni jooksul.</span><span class="sxs-lookup"><span data-stu-id="8c521-p102">The time it takes the job to run depends on the number of changes to process. A large number of changes takes longer. The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="8c521-110">Rohkem infot kasutaja profiili sünkroonimise SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="8c521-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

