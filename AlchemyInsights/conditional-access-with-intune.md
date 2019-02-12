---
title: Juurdepääsu Intune'iga
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29935926"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="ae584-102">Juurdepääsu Intune'iga</span><span class="sxs-lookup"><span data-stu-id="ae584-102">Conditional Access with Intune</span></span>

<span data-ttu-id="ae584-103">Kasutades **Tingimusjuurdepääsu** Intune'iga nõuab 3 sammu:</span><span class="sxs-lookup"><span data-stu-id="ae584-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="ae584-p101">**Tingimusliku juurdepääsu poliitika** , mis määratleb, milliseid ressursse on kaitstud, ja millised tingimused peavad olema täidetud juurdepääsu nende ressursside loomine. Näiteks seade peab olema ühilduv enne ettevõtte e-posti.</span><span class="sxs-lookup"><span data-stu-id="ae584-p101">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="ae584-p102">Seadete, mis peavad olema täidetud enne seadme nõuetele **Vastavuse poliitika** loomine. Näiteks seade peab olema vähemalt 6-kohaline pin leiti nõuetele.</span><span class="sxs-lookup"><span data-stu-id="ae584-p102">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="ae584-p103">Tagada **Täitmise poliitika** ja **Tingimusliku juurdepääsu poliitika** on suunatud soovitud kasutajarühmade. See võib nõuda teostamise loomine Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ae584-p103">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="ae584-110">Loe lähemalt:</span><span class="sxs-lookup"><span data-stu-id="ae584-110">Read more:</span></span>
  
- [<span data-ttu-id="ae584-111">Tingimusliku juurdepääsu parimate tavade</span><span class="sxs-lookup"><span data-stu-id="ae584-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="ae584-112">Alustamine: juurdepääsu</span><span class="sxs-lookup"><span data-stu-id="ae584-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

