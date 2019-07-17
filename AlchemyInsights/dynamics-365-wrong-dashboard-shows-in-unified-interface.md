---
title: Dynamics 365 - vale armatuurlaual Dynamics 365 ühtne liides
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 6edf6fbae0174f3fa4d635c7a99e7daae1243b60
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/16/2019
ms.locfileid: "35747429"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="2819f-102">Vale armatuurlaual Dynamics 365 ühtne liides</span><span class="sxs-lookup"><span data-stu-id="2819f-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="2819f-103">On mitu põhjust, miks võite näha teise armatuurlaua kui ootate:</span><span class="sxs-lookup"><span data-stu-id="2819f-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="2819f-104">Kasutaja valib kasutaja vaikimisi armatuurlaual</span><span class="sxs-lookup"><span data-stu-id="2819f-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="2819f-105">Tavaliselt saate tuvastada kasutaja vaikimisi armatuurlaual määratakse, kui nupu **Set Default** näitab armatuurlaua käsuriba.</span><span class="sxs-lookup"><span data-stu-id="2819f-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="2819f-106">Kasutaja vaikimisi armatuurlaual alistab muud vaikimisi armatuurlauad isegi siis, kui kasutaja vaikimisi armatuurlaual pole praeguses rakenduses.</span><span class="sxs-lookup"><span data-stu-id="2819f-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="2819f-107">Tühista lahendusena kasutada oma vaikimisi armatuurlaual.</span><span class="sxs-lookup"><span data-stu-id="2819f-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="2819f-108">Luuakse armatuurlaud, isiklik.</span><span class="sxs-lookup"><span data-stu-id="2819f-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="2819f-109">Et armatuurlaud kasutaja vaikesätte seadmine.</span><span class="sxs-lookup"><span data-stu-id="2819f-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="2819f-110">Selle armatuurlaua kustutamine.</span><span class="sxs-lookup"><span data-stu-id="2819f-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="2819f-111">Sisukord asub armatuurlaua</span><span class="sxs-lookup"><span data-stu-id="2819f-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="2819f-112">On seatud organisatsiooni vaikimisi armatuurlaual, valige armatuurlaua ning "Määra nii Default" "Kohandada süsteemi".</span><span class="sxs-lookup"><span data-stu-id="2819f-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="2819f-113">Kuid määratletud sitemap disainer armatuurlaud on ülimuslik selle armatuurlaua, kui kasutajal on juurdepääs.</span><span class="sxs-lookup"><span data-stu-id="2819f-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="2819f-114">Et kasutajad vaadata määramist organisatsiooni vaikimisi armatuurlaual, saate:</span><span class="sxs-lookup"><span data-stu-id="2819f-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="2819f-115">Määrata selle armatuurlaua sitemap</span><span class="sxs-lookup"><span data-stu-id="2819f-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="2819f-116">Sisukord, mis on määratletud armatuurlaua juurdepääsu nende kasutajate jaoks</span><span class="sxs-lookup"><span data-stu-id="2819f-116">Remove access to the sitemap defined dashboard for those users</span></span>
