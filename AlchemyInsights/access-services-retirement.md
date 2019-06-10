---
title: Juurdepääs teenuste pensionile
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: f5a1e88e4443fdf43cdd4f07cf9e784810df7540
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34769433"
---
# <a name="access-services-retirement"></a><span data-ttu-id="3111e-102">Juurdepääs teenuste pensionile</span><span class="sxs-lookup"><span data-stu-id="3111e-102">Access services retirement</span></span>

<span data-ttu-id="3111e-103">Kui me algselt teatas MC97576, märts 2017 ja jätkas suhelda viimase aasta jooksul on juurdepääsuteenused on pensionile Office 365.</span><span class="sxs-lookup"><span data-stu-id="3111e-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="3111e-104">Järgmine etapp selles protsessis saab olema juurdepääs Web andmebaasidele, mida kasutama SharePointi loendid oma alusandmeid ladustamiseks eemaldamist.</span><span class="sxs-lookup"><span data-stu-id="3111e-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="3111e-105">**Kuidas see mind mõjutab?**</span><span class="sxs-lookup"><span data-stu-id="3111e-105">**How does this affect me?**</span></span>

<span data-ttu-id="3111e-106">Alates juuni 2019, me peatus loomine uue Accessi andmebaaside SharePoint Online ja teenuse ja ülejäänud rakendused sulgeda aprill 2020.</span><span class="sxs-lookup"><span data-stu-id="3111e-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="3111e-107">**Mida vaja valmistada selle muudatuse teha?**</span><span class="sxs-lookup"><span data-stu-id="3111e-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="3111e-108">Soovitame teil luua ettevõtte juurdepääsu veebiandmebaasid ülemineku kava.</span><span class="sxs-lookup"><span data-stu-id="3111e-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="3111e-109">Administraatorid saate hankida juurdepääsu rakendused, mis kasutavad saitide loendi [SharePointi juurdepääs rakenduse skanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) .</span><span class="sxs-lookup"><span data-stu-id="3111e-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span> 

<span data-ttu-id="3111e-110">On mitu võimalust rännata andmetele juurdepääsu web andmebaasid:</span><span class="sxs-lookup"><span data-stu-id="3111e-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="3111e-111">Juurdepääs kohaliku andmebaasi importimine (. ACCDB) või Exceli faili.</span><span class="sxs-lookup"><span data-stu-id="3111e-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="3111e-112">Samuti soovitame uurida Microsoft PowerApps alternatiivse platvormi luua veebi ja mobiilseadmete koodita ärilahendusi.</span><span class="sxs-lookup"><span data-stu-id="3111e-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>