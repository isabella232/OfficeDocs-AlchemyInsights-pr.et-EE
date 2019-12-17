---
title: Õiguste probleemid migreerimine
ms.author: pebaum
author: pebaum
ms.date: 9/18/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: cbec51a7-5513-4848-a9ae-cdf993e000a8
ms.openlocfilehash: 95bfbfdf002e457230479a860058c1cf7ab1f8c2
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054410"
---
# <a name="user-profile-and-photo-synchronization"></a><span data-ttu-id="9cfe3-102">Kasutajaprofiili ja fotode sünkroonimine</span><span class="sxs-lookup"><span data-stu-id="9cfe3-102">User Profile and Photo synchronization</span></span>

 <span data-ttu-id="9cfe3-103">**Profiili foto sünkroonimine** -kasutajad võivad märgata, et nende profiilifotot ei sünkroonis SharePointiga.</span><span class="sxs-lookup"><span data-stu-id="9cfe3-103">**Profile Photo Synchronization** - Users may notice that their profile photo is not synchronizing to SharePoint.</span></span> <span data-ttu-id="9cfe3-104">Või nad võisid proovida värskendada oma profiilifotot ja foto ilmub ikka vana foto.</span><span class="sxs-lookup"><span data-stu-id="9cfe3-104">Or, they may have tried to update their profile photo and the photo still appears as the old photo.</span></span> <span data-ttu-id="9cfe3-105">Et tagada profiili foto kuvatakse ootuspäraselt, kasutaja peab käivitama foto sünkroonimine.</span><span class="sxs-lookup"><span data-stu-id="9cfe3-105">To ensure the profile photo shows as expected, the user will need to initiate a photo sync.</span></span> 
  
<span data-ttu-id="9cfe3-106">Foto sünkroonimise protsessi kohta lisateabe saamiseks vaadake [teavet profiili pildi sünkroonimine Office 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span><span class="sxs-lookup"><span data-stu-id="9cfe3-106">For more information about the photo synchronization process, see [Information about profile picture synchronization in Office 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span></span>
  
- <span data-ttu-id="9cfe3-107">**Profiili sünkroonimine** -profiili sünkroonimise lõpuleviimiseks vajalik aeg sõltub muudatuste (töö) arvust, mida AD Imporditöö peab töötlema.</span><span class="sxs-lookup"><span data-stu-id="9cfe3-107">**Profile Synchronization** - The time that's required to complete a profile synchronization depends on the number of changes (work) the AD Import Job has to process.</span></span> <span data-ttu-id="9cfe3-108">Kui on palju muudatusi, ajastitöö on palju tööd teha, ja see võtab kauem, et muudatused kajastuvad kasutajaprofiili rakendus.</span><span class="sxs-lookup"><span data-stu-id="9cfe3-108">If there are many changes, the timer job has a lot of work to do, and it will take longer for the changes to be reflected in the User Profile Application.</span></span> <span data-ttu-id="9cfe3-109">Kui ajastitöö on väike hulk tööd teha, kajastuvad muudatused kasutajaprofiili rakenduses palju kiiremini.</span><span class="sxs-lookup"><span data-stu-id="9cfe3-109">If the timer job has a small volume of work to do, the changes will be reflected in the User Profile Application much faster.</span></span> 
  
<span data-ttu-id="9cfe3-110">Profiili sünkroonimise protsessi kohta lisateabe saamiseks vaadake [teavet Kasutajaprofiili sünkroonimise kohta SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span><span class="sxs-lookup"><span data-stu-id="9cfe3-110">For more information about the profile synchronization process, see [Information about user profile synchronization in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span></span>
    
- <span data-ttu-id="9cfe3-111">**Värskendage profiili Office Delve** -Delve kasutajad saavad hallata oma Office 365 profiili.</span><span class="sxs-lookup"><span data-stu-id="9cfe3-111">**Update Profile in Office Delve** - Delve users can manage their Office 365 Profile.</span></span> <span data-ttu-id="9cfe3-112">Lisateavet leiate teemast [Office Delve ' i profiili vaatamine ja värskendamine](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="9cfe3-112">For more information, see [View and Update your profile in Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>
    

