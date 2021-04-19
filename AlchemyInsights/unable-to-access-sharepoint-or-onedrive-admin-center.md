---
title: SharePointile või OneDrive'i halduskeskusele ei pääse juurde
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: 7ba4a9c6995c03dd21e0e1aa387e407d41a08fb1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824431"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a><span data-ttu-id="d0f18-102">SharePointile või OneDrive'i halduskeskusele ei pääse juurde</span><span class="sxs-lookup"><span data-stu-id="d0f18-102">Unable to access SharePoint or OneDrive admin center</span></span>

- <span data-ttu-id="d0f18-103">Kui teie SharePointi või OneDrive'i halduskeskuse saidile ei pääse juurde või see pole saadaval, võib ilmneda ajutine teenuseprobleem, mille korral kasutajatel esineb SharePointi saitidele või OneDrive'i sisule juurdepääsemisel aeg-ajalt viivitusi või navigeerimistõrkeid.</span><span class="sxs-lookup"><span data-stu-id="d0f18-103">If your SharePoint or OneDrive Admin center site is inaccessible or unavailable, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="d0f18-104">Kontrollige [teenuse seisundi armatuurlauda,](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) et näha, kas teie ettevõtet mõjutab.</span><span class="sxs-lookup"><span data-stu-id="d0f18-104">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

- <span data-ttu-id="d0f18-105">Üld- ja SharePointi administraatoritele tuleb määrata SharePointi litsents.</span><span class="sxs-lookup"><span data-stu-id="d0f18-105">Global and SharePoint admins need to be assigned a SharePoint license.</span></span> <span data-ttu-id="d0f18-106">Äsja loodud kontod, millele on äsja määratud SharePointi litsents või administraatoriroll, võivad sharePointile juurdepääsul ilmneda probleemid, näiteks "juurdepääs keelatud" või "kasutajat ei leitud".</span><span class="sxs-lookup"><span data-stu-id="d0f18-106">Newly created accounts just assigned with a SharePoint License or Admin role might experience issues accessing SharePoint, like "access denied" or "user not found."</span></span> <span data-ttu-id="d0f18-107">Meie süsteemides sünkroonimise lõpuleviimiseks andke vähemalt 24 tundi.</span><span class="sxs-lookup"><span data-stu-id="d0f18-107">Please give at least 24 hours for sync to complete across our systems.</span></span> <span data-ttu-id="d0f18-108">Mõistame, et 24 tundi võib tunduda pika ajana.</span><span class="sxs-lookup"><span data-stu-id="d0f18-108">We understand that 24 hours may seem like a long time.</span></span> <span data-ttu-id="d0f18-109">Paljudel juhtudel töötame juba lahenduse kallal.</span><span class="sxs-lookup"><span data-stu-id="d0f18-109">In many cases, we're already working on a solution.</span></span>

- <span data-ttu-id="d0f18-110">Õigustega identiteedihaldus[(PIM) kasutajatele](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)võidakse juurdepääs keelata, kui lubatud juurdepääsuaja aken on väga väike, lugege teemat [PIM-i kontodele juurdepääs keelatud.](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="d0f18-110">Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new))  users may receive access denied if allowed access time window is very small, see  [Access denied to PIM accounts](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).</span></span>