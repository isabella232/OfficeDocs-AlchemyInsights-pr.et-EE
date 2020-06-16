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
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750966"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="a2942-102">"Nõutav Alchemy Header H1, H2'd ei tööta."</span><span class="sxs-lookup"><span data-stu-id="a2942-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="a2942-103">Parimad tavad ja juhised Alchemy authoring:</span><span class="sxs-lookup"><span data-stu-id="a2942-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="a2942-104">**Ära pesasta Alchemy Insightsi kaustades**- see murrab URL-i struktuuri.</span><span class="sxs-lookup"><span data-stu-id="a2942-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="a2942-105">Me uurime selle parandamist.</span><span class="sxs-lookup"><span data-stu-id="a2942-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="a2942-106">**Kaustas AlchemyInsights** olevatel failidel peaksid olema väikefailinimed sidekriipsudega tühikute ex jaoks.</span><span class="sxs-lookup"><span data-stu-id="a2942-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="a2942-107">***kohtuvaidluste lubamist***.</span><span class="sxs-lookup"><span data-stu-id="a2942-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="a2942-108">Kaasake reegli ID või ämber ID [Alchemy partneri portaali](https://alchemyportal.azurewebsites.net) ms.custom väljale.</span><span class="sxs-lookup"><span data-stu-id="a2942-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="a2942-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="a2942-109">ex.</span></span> <span data-ttu-id="a2942-110">***ms.custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="a2942-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="a2942-111">Kasutage mallina selle faili ülaosas olevad ülejäänud metaandmed.</span><span class="sxs-lookup"><span data-stu-id="a2942-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="a2942-112">Liikuge [portaalis Alchemy Partner](https://alchemyportal.azurewebsites.net)jaotiseni **Kliendiülevaate tiitel:** ja kasutage seda ülevaate saamiseks oma H1-tiitli lähtepunktina.</span><span class="sxs-lookup"><span data-stu-id="a2942-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="a2942-113">Alchemy Insights peab olema ainult ühe H1 ülaosas või nad murda tootmises.</span><span class="sxs-lookup"><span data-stu-id="a2942-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="a2942-114">H2-d ei renderdata nii, et kasutage eraldi jaotiste tähistamiseks **paksu** või muid konventsioone.</span><span class="sxs-lookup"><span data-stu-id="a2942-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="a2942-115">Järgmisena täitke kehatekst, kasutades lehe Alchemy Rule (Kliendiülevaated) jaotises Kliendiülevaated olevat mustandit.</span><span class="sxs-lookup"><span data-stu-id="a2942-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="a2942-116">Täpploendid on korras</span><span class="sxs-lookup"><span data-stu-id="a2942-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="a2942-117">Nummerdatud loendid ka</span><span class="sxs-lookup"><span data-stu-id="a2942-117">Numbered lists too</span></span>
    1. <span data-ttu-id="a2942-118">**Bold** ja *kursiiv* on a-ok</span><span class="sxs-lookup"><span data-stu-id="a2942-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="a2942-119">Lingid peaksid alati olema kas **"lingid veebile"/ välised** või **sügavad lingid kasutajaliidese elementidele,** mitte sisemised lingid.</span><span class="sxs-lookup"><span data-stu-id="a2942-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="a2942-120">Pilte ei toetata praegu ametlikult, kuid see on teekaardil.</span><span class="sxs-lookup"><span data-stu-id="a2942-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="a2942-121">Ja see on tõesti juba natuke liiga pikk.</span><span class="sxs-lookup"><span data-stu-id="a2942-121">And this is really already a bit too long.</span></span> <span data-ttu-id="a2942-122">Parim tava on umbes 400 tähemärki ---------------------------------</span><span class="sxs-lookup"><span data-stu-id="a2942-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="a2942-123">Kui teie sisu on valmis, tõmmake see live filiaal.</span><span class="sxs-lookup"><span data-stu-id="a2942-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="a2942-124">Seejärel [Alchemy partner portaali](https://alchemyportal.azurewebsites.net) ja sisestage failinimi url-i väljale.</span><span class="sxs-lookup"><span data-stu-id="a2942-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 