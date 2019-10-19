---
title: Dynamics 365-vale armatuurlaud näitab Dynamics 365 ühendatud liides
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36528547"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="12309-102">Vale armatuurlaud näitab Dynamics 365 ühendatud liides</span><span class="sxs-lookup"><span data-stu-id="12309-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="12309-103">On mitu põhjust, miks võite näha teise armatuurlaua kui see, mida ootate:</span><span class="sxs-lookup"><span data-stu-id="12309-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="12309-104">Kasutaja on seadnud kasutaja vaikimisi armatuurlaud</span><span class="sxs-lookup"><span data-stu-id="12309-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="12309-105">Tavaliselt saate tuvastada kasutaja vaikimisi armatuurlaud on seatud kui vaikimisi nuppu **Sea** ei kuvata armatuurlaua käsuribal.</span><span class="sxs-lookup"><span data-stu-id="12309-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="12309-106">Kasutaja vaikimisi armatuurlaud alistab kõik muud vaikimisi armatuurlauad isegi siis, kui kasutaja vaikimisi armatuurlaud ei ole praeguses rakenduses.</span><span class="sxs-lookup"><span data-stu-id="12309-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="12309-107">Kasutage järgmist lahendust, et Tühista oma vaikimisi armatuurlaud.</span><span class="sxs-lookup"><span data-stu-id="12309-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="12309-108">Saate luua uue isikliku armatuurlaua.</span><span class="sxs-lookup"><span data-stu-id="12309-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="12309-109">Seadke see uus armatuurlaud kasutaja vaikesätteks.</span><span class="sxs-lookup"><span data-stu-id="12309-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="12309-110">Kustutage armatuurlaud.</span><span class="sxs-lookup"><span data-stu-id="12309-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="12309-111">Armatuurlaud on seatud saidikaardi</span><span class="sxs-lookup"><span data-stu-id="12309-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="12309-112">Võimalik, et olete seadistanud organisatsiooni vaike-armatuurlaua, valides armatuurlaua ja valides jaotises "Kohanda süsteemi".</span><span class="sxs-lookup"><span data-stu-id="12309-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="12309-113">Kuid saidikaardi kujundajas määratletud armatuurlaud on selle armatuurlaua suhtes ülimuslik, kui kasutajal on sellele juurdepääs.</span><span class="sxs-lookup"><span data-stu-id="12309-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="12309-114">Kui soovite, et kasutajad näeksid armatuurlauda, mille olete seadnud organisatsiooni vaikesätteks, saate teha järgmist:</span><span class="sxs-lookup"><span data-stu-id="12309-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="12309-115">Armatuurlaua seadmine saidikaardi</span><span class="sxs-lookup"><span data-stu-id="12309-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="12309-116">Eemalda juurdepääs saidikaardi määratud armatuurlauale nende kasutajate jaoks</span><span class="sxs-lookup"><span data-stu-id="12309-116">Remove access to the sitemap defined dashboard for those users</span></span>
