---
title: Andmete asukoht
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655278"
---
# <a name="data-location"></a><span data-ttu-id="e60fe-102">Andmete asukoht</span><span class="sxs-lookup"><span data-stu-id="e60fe-102">Data location</span></span>

<span data-ttu-id="e60fe-103">Saate vaadata oma rentniku asukoht administreerimiskeskuses või ühendust Exchange Online PowerShelli kaudu.</span><span class="sxs-lookup"><span data-stu-id="e60fe-103">You can view the location of your tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="e60fe-104">**Halduskeskus:**</span><span class="sxs-lookup"><span data-stu-id="e60fe-104">**Admin center:**</span></span>
1. <span data-ttu-id="e60fe-105">Logige sisse [administreerimiskeskusesse](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="e60fe-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="e60fe-106">Valige **sätted** > **organisatsiooni profiil**.</span><span class="sxs-lookup"><span data-stu-id="e60fe-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="e60fe-107">Valige jaotises **andmete asukoht** **Kuva üksikasjad**.</span><span class="sxs-lookup"><span data-stu-id="e60fe-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="e60fe-108">**Powershelli:**</span><span class="sxs-lookup"><span data-stu-id="e60fe-108">**PowerShell:**</span></span>
1. <span data-ttu-id="e60fe-109">Windows PowerShelli abil ühendust Exchange Online ' i.</span><span class="sxs-lookup"><span data-stu-id="e60fe-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="e60fe-110">Käivitage cmdlet [-käsu Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) , et kuvada teie rentniku atribuutide loend.</span><span class="sxs-lookup"><span data-stu-id="e60fe-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant's properties.</span></span> 
3. <span data-ttu-id="e60fe-111">Vaadake atribuuti OrganizationId.</span><span class="sxs-lookup"><span data-stu-id="e60fe-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="e60fe-112">Kui teil on EXO ja SPO andmete asukoht, saate määrata andmete asukoha muude teenuste kohta, mida te [oma andmete](https://products.office.com/where-is-your-data-located)asukoha puhul kasutada võite.</span><span class="sxs-lookup"><span data-stu-id="e60fe-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>