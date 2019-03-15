---
title: 'sama faili nimi on parim [reegel #-kirjeldus]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e248c2ee3cbb9a86f21c1f36be10c893df76ff52
ms.sourcegitcommit: 3070905131e6d8449981231a3551c0bb4ca38ae6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30634500"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="1f41b-102">Nõutav alkeemia päise H1, H2's ei tööta.</span><span class="sxs-lookup"><span data-stu-id="1f41b-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="1f41b-103">Heade tavade ja suuniste alkeemia authoring:</span><span class="sxs-lookup"><span data-stu-id="1f41b-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="1f41b-104">**Pesa alkeemia ülevaatlikke kaustad**- see rikub URL-i struktuuri.</span><span class="sxs-lookup"><span data-stu-id="1f41b-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="1f41b-105">Ootame, millega seda arvesse.</span><span class="sxs-lookup"><span data-stu-id="1f41b-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="1f41b-106">Failid kaustas **AlchemyInsights** peaks olema reegli ID ja [alkeemia partneriportaal](https://alchemyportal.azurewebsites.net) reegli nimi faili nimi.</span><span class="sxs-lookup"><span data-stu-id="1f41b-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="1f41b-107">ex.</span><span class="sxs-lookup"><span data-stu-id="1f41b-107">ex.</span></span> <span data-ttu-id="1f41b-108">***976-How-to-enable-Litigation-Hold***</span><span class="sxs-lookup"><span data-stu-id="1f41b-108">***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="1f41b-109">Kasutada seda faili ülaosas metaandmete malli.</span><span class="sxs-lookup"><span data-stu-id="1f41b-109">Use the metadata at the top of this file as your template.</span></span> <span data-ttu-id="1f41b-110">Midagi ei ole vaja.</span><span class="sxs-lookup"><span data-stu-id="1f41b-110">Nothing else is required.</span></span>
1. <span data-ttu-id="1f41b-111">[Portaal alkeemia Partner](https://alchemyportal.azurewebsites.net)navigeerida jaotiseni **kliendile ülevaate pealkiri:** ja kasutamine, et kohe alguses tuleb seadusandjal punkti oma H1 pealkiri tutvustus.</span><span class="sxs-lookup"><span data-stu-id="1f41b-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="1f41b-112">Alkeemia teadmisi peab olema ainult ühe H1 ülaosas või vaheaega tootmises.</span><span class="sxs-lookup"><span data-stu-id="1f41b-112">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="1f41b-113">H2s ei muuda nii kasutada **paksu** või teiste konventsioonidega tähenda eraldi.</span><span class="sxs-lookup"><span data-stu-id="1f41b-113">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="1f41b-114">Seejärel sisestage kasutades eelnõu materjali alkeemia reegel lehe jaotises klientide vaatenurki kehatekst</span><span class="sxs-lookup"><span data-stu-id="1f41b-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="1f41b-115">Täppidega on ilusad</span><span class="sxs-lookup"><span data-stu-id="1f41b-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="1f41b-116">Nummerdatud loendite liiga</span><span class="sxs-lookup"><span data-stu-id="1f41b-116">Numbered lists too</span></span>
    1. <span data-ttu-id="1f41b-117">**Rasvase** ja *kursiivkirja* on a-ok</span><span class="sxs-lookup"><span data-stu-id="1f41b-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="1f41b-118">Lingid tuleb alati kas **"web linke" / väline** või **sügav-viited Kasutajaliidese elemendid**, mitte sisemised lingid.</span><span class="sxs-lookup"><span data-stu-id="1f41b-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="1f41b-119">Ja see on tõesti juba natuke liiga pikk.</span><span class="sxs-lookup"><span data-stu-id="1f41b-119">And this is really already a bit too long.</span></span> <span data-ttu-id="1f41b-120">On umbes 400 tähemärki---</span><span class="sxs-lookup"><span data-stu-id="1f41b-120">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="1f41b-121">Kui teie sisu on valmis, tõmmake see live kontorisse.</span><span class="sxs-lookup"><span data-stu-id="1f41b-121">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="1f41b-122">Seejärel minge [alkeemia partneriportaal](https://alchemyportal.azurewebsites.net) ja sisestage faili nimi väljale.</span><span class="sxs-lookup"><span data-stu-id="1f41b-122">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="1f41b-123">Veenduge, et läbi vaadata ja avaldada teavet ütleb "Jah" ja seejärel käsku Update reegel.</span><span class="sxs-lookup"><span data-stu-id="1f41b-123">Make sure Insight reviewed and published says "yes" and then click Update Rule.</span></span> <span data-ttu-id="1f41b-124">**(See näeb ilusam portaal - vabastades kiiresti uues versioonis.)** 
 ![URL-i väljale](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="1f41b-124">**(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

