---
title: 'sama faili nimi on parim [reegel #-kirjeldus]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 1bb1cb35f06e16a2dc85b7e2642b9fa0d203945e
ms.sourcegitcommit: b032c2ac45540b1eb5dd68a4ec7ce1a5d6922f0e
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29662926"
---
# <a name="required-customer-facing-h1-h2-doesnt-work"></a><span data-ttu-id="59743-102">Vajalik kliendi ees H1, H2 ei tööta</span><span class="sxs-lookup"><span data-stu-id="59743-102">Required Customer Facing H1, H2 doesn't work</span></span>
<span data-ttu-id="59743-103">Näitetekst blokeerida - järgige neid juhiseid:</span><span class="sxs-lookup"><span data-stu-id="59743-103">Example text block - follow these instructions:</span></span>

1. <span data-ttu-id="59743-104">Failid kaustas **AlchemyInsights** peaks olema reegli ID ja [alkeemia partneriportaal](https://alchemyportal.azurewebsites.net) reegli nimi faili nimi.</span><span class="sxs-lookup"><span data-stu-id="59743-104">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="59743-p101">nt ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="59743-p101">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="59743-p102">Kasutada seda faili ülaosas metaandmete malli. Midagi ei ole vaja.</span><span class="sxs-lookup"><span data-stu-id="59743-p102">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="59743-109">[Portaal alkeemia Partner](https://alchemyportal.azurewebsites.net)navigeerida jaotiseni **kliendile ülevaate pealkiri:** ja kasutamine, et kohe alguses tuleb seadusandjal punkti oma H1 pealkiri tutvustus.</span><span class="sxs-lookup"><span data-stu-id="59743-109">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="59743-p103">Alkeemia teadmisi peab olema ainult ühe H1 ülaosas või vaheaega tootmises. H2s ei muuda nii kasutada **paksu** või teiste konventsioonidega tähenda eraldi.</span><span class="sxs-lookup"><span data-stu-id="59743-p103">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="59743-112">Seejärel sisestage kasutades eelnõu materjali alkeemia reegel lehe jaotises klientide vaatenurki kehatekst</span><span class="sxs-lookup"><span data-stu-id="59743-112">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="59743-113">Täppidega on ilusad</span><span class="sxs-lookup"><span data-stu-id="59743-113">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="59743-114">Nummerdatud loendite liiga</span><span class="sxs-lookup"><span data-stu-id="59743-114">Numbered lists too</span></span>
    1. <span data-ttu-id="59743-115">**Rasvase** ja *kursiivkirja* on a-ok</span><span class="sxs-lookup"><span data-stu-id="59743-115">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="59743-116">Lingid tuleb alati kas **"web linke" / väline** või **sügav-viited Kasutajaliidese elemendid**, mitte sisemised lingid.</span><span class="sxs-lookup"><span data-stu-id="59743-116">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="59743-p104">Ja see on tõesti juba natuke liiga pikk. On umbes 400 tähemärki---</span><span class="sxs-lookup"><span data-stu-id="59743-p104">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="59743-p105">Kui teie sisu on valmis, tõmmake see live kontorisse. Seejärel minge [alkeemia partneriportaal](https://alchemyportal.azurewebsites.net) ja sisestage faili nimi väljale. Veenduge, et läbi vaadata ja avaldada teavet ütleb "Jah" ja seejärel käsku Update reegel. (See näeb ilusam uues versioonis portaali - vabastades kiiresti.)</span><span class="sxs-lookup"><span data-stu-id="59743-p105">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. (This will look prettier in the new version of the portal - releasing soon.)</span></span>

![URL-i väljale](media/for-content-team.PNG)

