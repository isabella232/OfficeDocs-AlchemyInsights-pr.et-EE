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
ms.openlocfilehash: 01d8b03209e734f1218de61d964524b1b9e1d044
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29939281"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="e8d2a-102">Nõutav alkeemia päise H1, H2's ei tööta.</span><span class="sxs-lookup"><span data-stu-id="e8d2a-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="e8d2a-103">Heade tavade ja suuniste alkeemia authoring:</span><span class="sxs-lookup"><span data-stu-id="e8d2a-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="e8d2a-p101">**Pesa alkeemia ülevaatlikke kaustad**- see rikub URL-i struktuuri. Ootame, millega seda arvesse.</span><span class="sxs-lookup"><span data-stu-id="e8d2a-p101">**Do not nest Alchemy Insights in folders**- this will break the url structure. We're looking into fixing this.</span></span>
1. <span data-ttu-id="e8d2a-106">Failid kaustas **AlchemyInsights** peaks olema reegli ID ja [alkeemia partneriportaal](https://alchemyportal.azurewebsites.net) reegli nimi faili nimi.</span><span class="sxs-lookup"><span data-stu-id="e8d2a-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="e8d2a-p102">nt ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="e8d2a-p102">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="e8d2a-p103">Kasutada seda faili ülaosas metaandmete malli. Midagi ei ole vaja.</span><span class="sxs-lookup"><span data-stu-id="e8d2a-p103">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="e8d2a-111">[Portaal alkeemia Partner](https://alchemyportal.azurewebsites.net)navigeerida jaotiseni **kliendile ülevaate pealkiri:** ja kasutamine, et kohe alguses tuleb seadusandjal punkti oma H1 pealkiri tutvustus.</span><span class="sxs-lookup"><span data-stu-id="e8d2a-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="e8d2a-p104">Alkeemia teadmisi peab olema ainult ühe H1 ülaosas või vaheaega tootmises. H2s ei muuda nii kasutada **paksu** või teiste konventsioonidega tähenda eraldi.</span><span class="sxs-lookup"><span data-stu-id="e8d2a-p104">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="e8d2a-114">Seejärel sisestage kasutades eelnõu materjali alkeemia reegel lehe jaotises klientide vaatenurki kehatekst</span><span class="sxs-lookup"><span data-stu-id="e8d2a-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="e8d2a-115">Täppidega on ilusad</span><span class="sxs-lookup"><span data-stu-id="e8d2a-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="e8d2a-116">Nummerdatud loendite liiga</span><span class="sxs-lookup"><span data-stu-id="e8d2a-116">Numbered lists too</span></span>
    1. <span data-ttu-id="e8d2a-117">**Rasvase** ja *kursiivkirja* on a-ok</span><span class="sxs-lookup"><span data-stu-id="e8d2a-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="e8d2a-118">Lingid tuleb alati kas **"web linke" / väline** või **sügav-viited Kasutajaliidese elemendid**, mitte sisemised lingid.</span><span class="sxs-lookup"><span data-stu-id="e8d2a-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="e8d2a-p105">Ja see on tõesti juba natuke liiga pikk. On umbes 400 tähemärki---</span><span class="sxs-lookup"><span data-stu-id="e8d2a-p105">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="e8d2a-p106">Kui teie sisu on valmis, tõmmake see live kontorisse. Seejärel minge [alkeemia partneriportaal](https://alchemyportal.azurewebsites.net) ja sisestage faili nimi väljale. Veenduge, et läbi vaadata ja avaldada teavet ütleb "Jah" ja seejärel käsku Update reegel. **(See näeb ilusam uues versioonis portaali - vabastades kiiresti.)** 
 ![URL-i väljale](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="e8d2a-p106">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. **(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

