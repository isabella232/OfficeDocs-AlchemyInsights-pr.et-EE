---
title: sama, mis failinimi on parim
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e2dcca1295e37007593b34c2d818ad1d1133e4a1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676529"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="bdcf4-102">Nõutav Alchemy päis H1, H2's ei tööta.</span><span class="sxs-lookup"><span data-stu-id="bdcf4-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="bdcf4-103">Alchemy loome parimad tavad ja suunised:</span><span class="sxs-lookup"><span data-stu-id="bdcf4-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="bdcf4-104">**Ära pesa Alchemy ülevaated kaustades**-See murrab URL-i struktuuri.</span><span class="sxs-lookup"><span data-stu-id="bdcf4-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="bdcf4-105">Me otsime seda.</span><span class="sxs-lookup"><span data-stu-id="bdcf4-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="bdcf4-106">Kaustas **Alchemyinvaatamisväärsuste** failid peaksid olema väiketäide failinimed sidekriipsu ruumid ex.</span><span class="sxs-lookup"><span data-stu-id="bdcf4-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="bdcf4-107">***Kuidas lubada-kohtuvaidluste ootel***.</span><span class="sxs-lookup"><span data-stu-id="bdcf4-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="bdcf4-108">Lisage MS. Custom väljal [Alchemy partneri portaalist](https://alchemyportal.azurewebsites.net) reegli ID või jääkfailihulga ID.</span><span class="sxs-lookup"><span data-stu-id="bdcf4-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="bdcf4-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="bdcf4-109">ex.</span></span> <span data-ttu-id="bdcf4-110">***MS Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="bdcf4-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="bdcf4-111">Kasutage oma mallina selle faili ülaosas olevaid ülejäänud metaandmeid.</span><span class="sxs-lookup"><span data-stu-id="bdcf4-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="bdcf4-112">Liikuge [Alchemy Partneriportaalis](https://alchemyportal.azurewebsites.net)alla jaotisse **Kliendi ülevaate tiitel:** ja kasutage seda, et lähtepunktiks oma H1 pealkiri ülevaate saamiseks.</span><span class="sxs-lookup"><span data-stu-id="bdcf4-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="bdcf4-113">Alchemy Insights peab olema ainult üks H1 ülaosas või nad murravad tootmises.</span><span class="sxs-lookup"><span data-stu-id="bdcf4-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="bdcf4-114">H2s ei muuda nii **bold** kui ka muude konventsioonide kasutamist eraldi sektsioonideks.</span><span class="sxs-lookup"><span data-stu-id="bdcf4-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="bdcf4-115">Järgmisena täitke kehatekst, kasutades materjali mustandit Alchemy reegli lehe jaotises Kliendiülevaated</span><span class="sxs-lookup"><span data-stu-id="bdcf4-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="bdcf4-116">Täpp loendid on korras</span><span class="sxs-lookup"><span data-stu-id="bdcf4-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="bdcf4-117">Nummerdatud loendid on liiga</span><span class="sxs-lookup"><span data-stu-id="bdcf4-117">Numbered lists too</span></span>
    1. <span data-ttu-id="bdcf4-118">**Paks** ja *kursiiv* on-OK</span><span class="sxs-lookup"><span data-stu-id="bdcf4-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="bdcf4-119">Lingid peaksid alati olema kas **"lingid veebi"/välised** või **Deep-lingid UI elemendid**, mitte sisemine lingid.</span><span class="sxs-lookup"><span data-stu-id="bdcf4-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="bdcf4-120">Pilte ei toetata praegu ametlikult, kuid see on teekaardi peal.</span><span class="sxs-lookup"><span data-stu-id="bdcf4-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="bdcf4-121">Ja see on juba natuke liiga pikk.</span><span class="sxs-lookup"><span data-stu-id="bdcf4-121">And this is really already a bit too long.</span></span> <span data-ttu-id="bdcf4-122">Parim tava on umbes 400 tähemärki---------------------------------</span><span class="sxs-lookup"><span data-stu-id="bdcf4-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="bdcf4-123">Kui teie sisu on valmis, tõmmake see Live haru.</span><span class="sxs-lookup"><span data-stu-id="bdcf4-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="bdcf4-124">Seejärel [Alchemy partneri portaali](https://alchemyportal.azurewebsites.net) ja sisestage failinimi URL-i väljale.</span><span class="sxs-lookup"><span data-stu-id="bdcf4-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 