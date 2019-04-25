---
title: Profiilisünkroonimise
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: d1a72a85767e36fefbfa8eee266befcaf2e48af0
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371980"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="53782-102">Kuna minu profiili muudatused sünkroonida SharePointi kasutajaprofiili rakendusel?</span><span class="sxs-lookup"><span data-stu-id="53782-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="53782-103">SharePoint Online kasutab Active Directory importimine ajastitöö (AD Import) importimiseks kasutaja profiili rakenduse kasutajad ja rühmad.</span><span class="sxs-lookup"><span data-stu-id="53782-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="53782-104">AD impordi sünkroonib muudatused SharePoint Online kataloogi poest kasutajaprofiili rakendusel.</span><span class="sxs-lookup"><span data-stu-id="53782-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="53782-105">Need muutused jõustuvad partiina.</span><span class="sxs-lookup"><span data-stu-id="53782-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="53782-106">Ajastitöö töötab kuni muudatused on sünkroonitud.</span><span class="sxs-lookup"><span data-stu-id="53782-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="53782-107">Töö, mis käivitatakse kuluv aeg sõltub muutuste protsessi.</span><span class="sxs-lookup"><span data-stu-id="53782-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="53782-108">Mitmeid muudatusi võtab kauem aega.</span><span class="sxs-lookup"><span data-stu-id="53782-108">A large number of changes takes longer.</span></span> <span data-ttu-id="53782-109">Teenuse teenindustaseme lepingut (SLA) märgib, et SharePoint Online kataloogis kasutaja muutmine kajastub kasutajaprofiili rakendusel 24 tunni jooksul.</span><span class="sxs-lookup"><span data-stu-id="53782-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="53782-110">Rohkem infot kasutaja profiili sünkroonimise SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="53782-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

