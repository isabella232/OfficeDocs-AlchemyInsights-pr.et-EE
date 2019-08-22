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
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36504990"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="f079f-102">Juurdepääsu Intune'iga</span><span class="sxs-lookup"><span data-stu-id="f079f-102">Conditional Access with Intune</span></span>

<span data-ttu-id="f079f-103">Kasutades **Tingimusjuurdepääsu** Intune'iga nõuab 3 sammu:</span><span class="sxs-lookup"><span data-stu-id="f079f-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="f079f-104">**Tingimusliku juurdepääsu poliitika** , mis määratleb, milliseid ressursse on kaitstud, ja millised tingimused peavad olema täidetud juurdepääsu nende ressursside loomine.</span><span class="sxs-lookup"><span data-stu-id="f079f-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="f079f-105">Näiteks seade peab olema ühilduv enne ettevõtte e-posti.</span><span class="sxs-lookup"><span data-stu-id="f079f-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="f079f-106">Seadete, mis peavad olema täidetud enne seadme nõuetele **Vastavuse poliitika** loomine.</span><span class="sxs-lookup"><span data-stu-id="f079f-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="f079f-107">Näiteks seade peab olema vähemalt 6-kohaline pin leiti nõuetele.</span><span class="sxs-lookup"><span data-stu-id="f079f-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="f079f-108">Tagada **Täitmise poliitika** ja **Tingimusliku juurdepääsu poliitika** on suunatud soovitud kasutajarühmade.</span><span class="sxs-lookup"><span data-stu-id="f079f-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="f079f-109">See võib nõuda teostamise loomine Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f079f-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="f079f-110">Loe lähemalt:</span><span class="sxs-lookup"><span data-stu-id="f079f-110">Read more:</span></span>
  
- [<span data-ttu-id="f079f-111">Tingimusliku juurdepääsu parimate tavade</span><span class="sxs-lookup"><span data-stu-id="f079f-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="f079f-112">Alustamine: juurdepääsu</span><span class="sxs-lookup"><span data-stu-id="f079f-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

