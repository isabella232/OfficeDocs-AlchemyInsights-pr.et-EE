---
title: Profiili sünkroonimine
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36554329"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="6e34e-102">Millal muudab profiil SharePointi kasutajaprofiili rakenduse sünkroonimist?</span><span class="sxs-lookup"><span data-stu-id="6e34e-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="6e34e-103">SharePoint Online kasutab Active Directory importimine ajastitöö (AD import) kasutajate ja rühmade importimiseks kasutajaprofiili rakendusse.</span><span class="sxs-lookup"><span data-stu-id="6e34e-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="6e34e-104">AD impordi sünkroonib muudatused SharePoint Online ' i Kataloogipoest kasutajaprofiili rakendus.</span><span class="sxs-lookup"><span data-stu-id="6e34e-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="6e34e-105">Neid muudatusi töödeldakse partiidena.</span><span class="sxs-lookup"><span data-stu-id="6e34e-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="6e34e-106">Ajastitöö töötab seni, kuni muudatused sünkroonitakse.</span><span class="sxs-lookup"><span data-stu-id="6e34e-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="6e34e-107">Töö käivitamiseks kuluv aeg sõltub protsessi muutuste arvust.</span><span class="sxs-lookup"><span data-stu-id="6e34e-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="6e34e-108">Suur hulk muudatusi võtab kauem aega.</span><span class="sxs-lookup"><span data-stu-id="6e34e-108">A large number of changes takes longer.</span></span> <span data-ttu-id="6e34e-109">Teenusetaseme leping (SLA) teatab, et kasutaja SharePoint Online ' i kataloogi muutmine kajastub kasutajaprofiili rakenduse 24 tunni jooksul.</span><span class="sxs-lookup"><span data-stu-id="6e34e-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="6e34e-110">Rohkem infot Kasutajaprofiili sünkroonimise kohta SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="6e34e-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

