---
title: Tingimuslik juurdepääs Intune ' iga
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706017"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="22c21-102">Tingimuslik juurdepääs Intune ' iga</span><span class="sxs-lookup"><span data-stu-id="22c21-102">Conditional Access with Intune</span></span>

<span data-ttu-id="22c21-103">**Tingimusliku juurdepääsu** kasutamine Intune ' iga nõuab 3 etappi:</span><span class="sxs-lookup"><span data-stu-id="22c21-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="22c21-104">Looge **tingimuslik juurdepääsupoliitika** , mis määratleb, milliseid ressursse kaitstakse, ja millised tingimused peavad neile ressurssidele juurdepääsuks vastama.</span><span class="sxs-lookup"><span data-stu-id="22c21-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="22c21-105">Näiteks seade peab olema ühilduv enne juurdepääsu ettevõtte e-posti.</span><span class="sxs-lookup"><span data-stu-id="22c21-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="22c21-106">Looge **Vastavuspoliitika** , et määratleda sätted, mis peavad olema täidetud enne seadme ühildumist.</span><span class="sxs-lookup"><span data-stu-id="22c21-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="22c21-107">Näiteks peab seadmel olema vähemalt 6-kohaline PIN-kood, enne kui seda peetakse vastavaks.</span><span class="sxs-lookup"><span data-stu-id="22c21-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="22c21-108">**Nõuetele vastavuse poliitika** ja **tingimuslike juurdepääsupoliitikate** tagamine on suunatud soovitud kasutajate rühmadele.</span><span class="sxs-lookup"><span data-stu-id="22c21-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="22c21-109">See võib nõuda teatud kasutajate rühmade loomine Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="22c21-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="22c21-110">Loe lähemalt:</span><span class="sxs-lookup"><span data-stu-id="22c21-110">Read more:</span></span>
  
- [<span data-ttu-id="22c21-111">Tingimuslike juurdepääsu parimad tavad</span><span class="sxs-lookup"><span data-stu-id="22c21-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="22c21-112">Tingimusliku juurdepääsuga alustamine</span><span class="sxs-lookup"><span data-stu-id="22c21-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

