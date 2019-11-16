---
title: Juurdepääs teenustele pensionile
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 11/15/2019
ms.locfileid: "36747780"
---
# <a name="access-services-retirement"></a><span data-ttu-id="6e469-102">Juurdepääs teenustele pensionile</span><span class="sxs-lookup"><span data-stu-id="6e469-102">Access services retirement</span></span>

<span data-ttu-id="6e469-103">Nagu me algselt teatas MC97576, märtsis 2017, ja jätkas suhtlemine viimase aasta juurdepääsuteenused on pensionile Office 365.</span><span class="sxs-lookup"><span data-stu-id="6e469-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="6e469-104">Järgmise etapi selle protsessi on eemaldamine Access Web andmebaasid, mis kasutavad SharePointi loendid nende aluseks andmete salvestamise.</span><span class="sxs-lookup"><span data-stu-id="6e469-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="6e469-105">**Kuidas see mind mõjutab?**</span><span class="sxs-lookup"><span data-stu-id="6e469-105">**How does this affect me?**</span></span>

<span data-ttu-id="6e469-106">Alates juunist 2019, me peatada uute Accessi andmebaaside loomine SharePoint Online ' i ja sulgege teenus ja kõik ülejäänud rakendused aprill 2020.</span><span class="sxs-lookup"><span data-stu-id="6e469-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="6e469-107">**Mida ma pean tegema, et selleks muutusega valmistuda?**</span><span class="sxs-lookup"><span data-stu-id="6e469-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="6e469-108">Soovitame luua oma organisatsiooni Accessi veebiandmebaasidele üleminekuplaani.</span><span class="sxs-lookup"><span data-stu-id="6e469-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="6e469-109">Administraatorid saavad kasutada [SharePoint Accessi rakenduse skannerit](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) , et hankida saitide kasutamisel Accessi rakendusi.</span><span class="sxs-lookup"><span data-stu-id="6e469-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="6e469-110">Accessi veebiandmebaaside andmete migreerimiseks on mitu võimalust.</span><span class="sxs-lookup"><span data-stu-id="6e469-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="6e469-111">Importimine kohalikku Accessi andmebaasi (. ACCDB) või Exceli faili.</span><span class="sxs-lookup"><span data-stu-id="6e469-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="6e469-112">Samuti soovitame uurida Microsoft PowerApps alternatiivse platvormina luua koodi Business lahendusi veebi-ja mobiilsideseadmete.</span><span class="sxs-lookup"><span data-stu-id="6e469-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>