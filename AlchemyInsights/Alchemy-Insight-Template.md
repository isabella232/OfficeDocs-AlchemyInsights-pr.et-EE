---
title: sama faili nimi on parim
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: b77e514da36701808d46248e8f2a45137751a1c7
ms.sourcegitcommit: 5447031f9d0a320c49897b8adb5d29ac9437fbc5
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/18/2019
ms.locfileid: "35786409"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="46e38-102">Nõutav alkeemia päise H1, H2's ei tööta.</span><span class="sxs-lookup"><span data-stu-id="46e38-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="46e38-103">Heade tavade ja suuniste alkeemia authoring:</span><span class="sxs-lookup"><span data-stu-id="46e38-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="46e38-104">**Pesa alkeemia ülevaatlikke kaustad**- see rikub URL-i struktuuri.</span><span class="sxs-lookup"><span data-stu-id="46e38-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="46e38-105">Ootame, millega seda arvesse.</span><span class="sxs-lookup"><span data-stu-id="46e38-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="46e38-106">Failid kaustas **AlchemyInsights** peaks olema väike failinimesid ruumid ex sidekriipsudega.</span><span class="sxs-lookup"><span data-stu-id="46e38-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="46e38-107">***Kuidas-to-luba-otsuse-ootel***.</span><span class="sxs-lookup"><span data-stu-id="46e38-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="46e38-108">Reegli ID või ämber ID: [alkeemia partneriportaal](https://alchemyportal.azurewebsites.net) kaasata ms.custom välja.</span><span class="sxs-lookup"><span data-stu-id="46e38-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="46e38-109">ex.</span><span class="sxs-lookup"><span data-stu-id="46e38-109">ex.</span></span> <span data-ttu-id="46e38-110">***MS.Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="46e38-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="46e38-111">Kasutada ülejäänud metaandmete faili ülaosas malli.</span><span class="sxs-lookup"><span data-stu-id="46e38-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="46e38-112">[Portaal alkeemia Partner](https://alchemyportal.azurewebsites.net)navigeerida jaotiseni **kliendile ülevaate pealkiri:** ja kasutamine, et kohe alguses tuleb seadusandjal punkti oma H1 pealkiri tutvustus.</span><span class="sxs-lookup"><span data-stu-id="46e38-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="46e38-113">Alkeemia teadmisi peab olema ainult ühe H1 ülaosas või vaheaega tootmises.</span><span class="sxs-lookup"><span data-stu-id="46e38-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="46e38-114">H2s ei muuda nii kasutada **paksu** või teiste konventsioonidega tähenda eraldi.</span><span class="sxs-lookup"><span data-stu-id="46e38-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="46e38-115">Seejärel sisestage kasutades eelnõu materjali alkeemia reegel lehe jaotises klientide vaatenurki kehatekst</span><span class="sxs-lookup"><span data-stu-id="46e38-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="46e38-116">Täppidega on ilusad</span><span class="sxs-lookup"><span data-stu-id="46e38-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="46e38-117">Nummerdatud loendite liiga</span><span class="sxs-lookup"><span data-stu-id="46e38-117">Numbered lists too</span></span>
    1. <span data-ttu-id="46e38-118">**Rasvase** ja *kursiivkirja* on a-ok</span><span class="sxs-lookup"><span data-stu-id="46e38-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="46e38-119">Lingid tuleb alati kas **"web linke" / väline** või **sügav-viited Kasutajaliidese elemendid**, mitte sisemised lingid.</span><span class="sxs-lookup"><span data-stu-id="46e38-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="46e38-120">Pildid ei toeta praegu, kuid see on peal.</span><span class="sxs-lookup"><span data-stu-id="46e38-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="46e38-121">Ja see on tõesti juba natuke liiga pikk.</span><span class="sxs-lookup"><span data-stu-id="46e38-121">And this is really already a bit too long.</span></span> <span data-ttu-id="46e38-122">On umbes 400 tähemärki---</span><span class="sxs-lookup"><span data-stu-id="46e38-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="46e38-123">Kui teie sisu on valmis, tõmmake see live kontorisse.</span><span class="sxs-lookup"><span data-stu-id="46e38-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="46e38-124">Seejärel minge [alkeemia partneriportaal](https://alchemyportal.azurewebsites.net) ja sisestage faili nimi väljale.</span><span class="sxs-lookup"><span data-stu-id="46e38-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 


