---
title: Dynamics 365 – vale armatuurlaud kuvatakse rakenduses Dynamics 365 Unified Interface
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711271"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="b4677-102">Rakenduses Dynamics 365 Unified Interface kuvatakse valed armatuurlauad</span><span class="sxs-lookup"><span data-stu-id="b4677-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="b4677-103">On mitu põhjust, miks võidakse kuvada mõni muu armatuurlaud kui see, mida ootate.</span><span class="sxs-lookup"><span data-stu-id="b4677-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="b4677-104">Kasutaja on määranud kasutaja vaike-armatuurlaua.</span><span class="sxs-lookup"><span data-stu-id="b4677-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="b4677-105">Tavaliselt saate määrata kasutaja vaike-armatuurlaua, kui nupp **Sea vaikesätteks** ei kuvata armatuurlaual.</span><span class="sxs-lookup"><span data-stu-id="b4677-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="b4677-106">Kasutaja vaike-armatuurlaud alistab kõik muud vaike-armatuurlauad, isegi kui kasutaja vaike-armatuurlaud pole praeguses rakenduses.</span><span class="sxs-lookup"><span data-stu-id="b4677-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="b4677-107">Kasutage järgmisi lahendusi, et Andmebaasiparooli tühistamine nende vaike-armatuurlaud.</span><span class="sxs-lookup"><span data-stu-id="b4677-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="b4677-108">Saate luua uue isikliku armatuurlaua.</span><span class="sxs-lookup"><span data-stu-id="b4677-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="b4677-109">Seadke uus armatuurlaud kasutaja vaikesätteks.</span><span class="sxs-lookup"><span data-stu-id="b4677-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="b4677-110">Armatuurlaua kustutamine.</span><span class="sxs-lookup"><span data-stu-id="b4677-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="b4677-111">Armatuurlaud on määratud sitemap-s</span><span class="sxs-lookup"><span data-stu-id="b4677-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="b4677-112">Võimalik, et olete määranud organisatsiooni vaike-armatuurlaua, valides armatuurlaua ja valides jaotises "süsteemi kohandamine" valiku "Määra vaikesätteks".</span><span class="sxs-lookup"><span data-stu-id="b4677-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="b4677-113">Kui kasutajal on juurdepääs sellele armatuurlauale, on sisukaarti kujundajas määratletud armatuurlaud ülimuslikud.</span><span class="sxs-lookup"><span data-stu-id="b4677-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="b4677-114">Kui soovite, et kasutajad näeksid armatuurlauda, mille olete määranud organisatsiooni vaikeprogrammiks, saate teha järgmist.</span><span class="sxs-lookup"><span data-stu-id="b4677-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="b4677-115">Armatuurlaua seadmine sisukorda</span><span class="sxs-lookup"><span data-stu-id="b4677-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="b4677-116">Juurdepääsu eemaldamine nende kasutajate jaoks mõeldud sitemap-i jaoks määratud armatuurlauale</span><span class="sxs-lookup"><span data-stu-id="b4677-116">Remove access to the sitemap defined dashboard for those users</span></span>
