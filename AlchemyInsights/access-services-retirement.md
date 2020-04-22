---
title: Juurdepääs teenustele pensionile
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 977bd5887ef58b328463a9befcd6b47ac55f5a85
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687254"
---
# <a name="access-services-retirement"></a><span data-ttu-id="88050-102">Juurdepääs teenustele pensionile</span><span class="sxs-lookup"><span data-stu-id="88050-102">Access services retirement</span></span>

<span data-ttu-id="88050-103">Nagu me algselt teatas MC97576, märtsis 2017, ja jätkas suhtlemine viimase aasta juurdepääsuteenused on pensionil.</span><span class="sxs-lookup"><span data-stu-id="88050-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="88050-104">Järgmise etapi selle protsessi on eemaldamine Access Web andmebaasid, mis kasutavad SharePointi loendid nende aluseks andmete salvestamise.</span><span class="sxs-lookup"><span data-stu-id="88050-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="88050-105">**Kuidas see mind mõjutab?**</span><span class="sxs-lookup"><span data-stu-id="88050-105">**How does this affect me?**</span></span>

<span data-ttu-id="88050-106">Alates juunist 2019, me peatada uute Accessi andmebaaside loomine SharePoint Online ' i ja sulgege teenus ja kõik ülejäänud rakendused aprill 2020.</span><span class="sxs-lookup"><span data-stu-id="88050-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="88050-107">**Mida ma pean tegema, et selleks muutusega valmistuda?**</span><span class="sxs-lookup"><span data-stu-id="88050-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="88050-108">Soovitame luua oma organisatsiooni Accessi veebiandmebaasidele üleminekuplaani.</span><span class="sxs-lookup"><span data-stu-id="88050-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="88050-109">Administraatorid saavad kasutada [SharePoint Accessi rakenduse skannerit](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) , et hankida saitide kasutamisel Accessi rakendusi.</span><span class="sxs-lookup"><span data-stu-id="88050-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="88050-110">Accessi veebiandmebaaside andmete migreerimiseks on mitu võimalust.</span><span class="sxs-lookup"><span data-stu-id="88050-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="88050-111">Importimine kohalikku Accessi andmebaasi (. ACCDB) või Exceli faili.</span><span class="sxs-lookup"><span data-stu-id="88050-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="88050-112">Samuti soovitame uurida Microsoft PowerApps alternatiivse platvormina luua koodi Business lahendusi veebi-ja mobiilsideseadmete.</span><span class="sxs-lookup"><span data-stu-id="88050-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>