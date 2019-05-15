---
title: Juurdepääs teenuste pensionile
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 395dac6abf1562aa0da0b1d87eddd943affefc3f
ms.sourcegitcommit: b2c9202b94fa1ce73dbeb3e43b219ba07e46e7e3
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/14/2019
ms.locfileid: "33973912"
---
# <a name="access-services-retirement"></a><span data-ttu-id="dd22b-102">Juurdepääs teenuste pensionile</span><span class="sxs-lookup"><span data-stu-id="dd22b-102">Access services retirement</span></span>

<span data-ttu-id="dd22b-103">Kui me algselt teatas MC97576, märts 2017 ja jätkas suhelda viimase aasta jooksul on juurdepääsuteenused on pensionile Office 365.</span><span class="sxs-lookup"><span data-stu-id="dd22b-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="dd22b-104">Järgmine etapp selles protsessis saab olema juurdepääs Web andmebaasidele, mida kasutama SharePointi loendid oma alusandmeid ladustamiseks eemaldamist.</span><span class="sxs-lookup"><span data-stu-id="dd22b-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

## <a name="how-does-this-affect-me"></a><span data-ttu-id="dd22b-105">Kuidas see mind mõjutab?</span><span class="sxs-lookup"><span data-stu-id="dd22b-105">How does this affect me?</span></span>

<span data-ttu-id="dd22b-106">Alates juuni 2019, me peatus loomine uue Accessi andmebaaside SharePoint Online ja teenuse ja ülejäänud rakendused sulgeda aprill 2020.</span><span class="sxs-lookup"><span data-stu-id="dd22b-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

## <a name="what-do-i-need-to-do-to-prepare-for-this-change"></a><span data-ttu-id="dd22b-107">Mida vaja valmistada selle muudatuse teha?</span><span class="sxs-lookup"><span data-stu-id="dd22b-107">What do I need to do to prepare for this change?</span></span>

<span data-ttu-id="dd22b-108">Soovitame teil luua ettevõtte juurdepääsu veebiandmebaasid ülemineku kava.</span><span class="sxs-lookup"><span data-stu-id="dd22b-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="dd22b-109">Administraatorid saate hankida juurdepääsu rakendused, mis kasutavad saitide loendi [SharePointi juurdepääs rakenduse skanner](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) .</span><span class="sxs-lookup"><span data-stu-id="dd22b-109">Admins can use the [SharePoint Access app scanner](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) to obtain an inventory of the Access apps that sites are using.</span></span> 

<span data-ttu-id="dd22b-110">On mitu võimalust rännata andmetele juurdepääsu web andmebaasid:</span><span class="sxs-lookup"><span data-stu-id="dd22b-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="dd22b-111">Juurdepääs kohaliku andmebaasi importimine (. ACCDB) või Exceli faili.</span><span class="sxs-lookup"><span data-stu-id="dd22b-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="dd22b-112">Samuti soovitame uurida Microsoft PowerApps alternatiivse platvormi luua veebi ja mobiilseadmete koodita ärilahendusi.</span><span class="sxs-lookup"><span data-stu-id="dd22b-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>