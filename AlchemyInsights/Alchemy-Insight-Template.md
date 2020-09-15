---
title: sama, mis failinimi on parim
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664130"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="fd9ec-102">"Nõutav alkeemia päis H1, H2's ei tööta."</span><span class="sxs-lookup"><span data-stu-id="fd9ec-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="fd9ec-103">Alkeemia autorluse head tavad ja juhised.</span><span class="sxs-lookup"><span data-stu-id="fd9ec-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="fd9ec-104">**Ära pesasta alkeemia-ülevaadet kaustadesse**– See murrab URL-i struktuuri.</span><span class="sxs-lookup"><span data-stu-id="fd9ec-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="fd9ec-105">Me otsime selle parandamist.</span><span class="sxs-lookup"><span data-stu-id="fd9ec-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="fd9ec-106">Kaustas **AlchemyInsights** olevatel failidel peaks olema väiksed failinimed sidekriipsuga tühikute jaoks.</span><span class="sxs-lookup"><span data-stu-id="fd9ec-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="fd9ec-107">***Kuidas-to-enable-kohtuvaidlus-ootel***.</span><span class="sxs-lookup"><span data-stu-id="fd9ec-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="fd9ec-108">Lisage reegli ID või ämber ID andmebaasi [alkeemia partner portaalist](https://alchemyportal.azurewebsites.net) MS. custom.</span><span class="sxs-lookup"><span data-stu-id="fd9ec-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="fd9ec-109">ex0.</span><span class="sxs-lookup"><span data-stu-id="fd9ec-109">ex.</span></span> <span data-ttu-id="fd9ec-110">***MS kohandatud: 100021***</span><span class="sxs-lookup"><span data-stu-id="fd9ec-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="fd9ec-111">Kasutage mallina selle lehe ülaosas olevat ülejäänud metaandmeid.</span><span class="sxs-lookup"><span data-stu-id="fd9ec-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="fd9ec-112">Jaotises [Alchemy partnerite portaal](https://alchemyportal.azurewebsites.net)saate liikuda jaotise **Kliendi ülevaate pealkiri:** ja kasutada seda, kui soovite, et teie H1 pealkiri oleks lähtepunkt.</span><span class="sxs-lookup"><span data-stu-id="fd9ec-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="fd9ec-113">Alkeemia-ülevaadetel peab ülaosas olema ainult üks H1 või see puruneb tootmisel.</span><span class="sxs-lookup"><span data-stu-id="fd9ec-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="fd9ec-114">H2s ei saa muuta nii **paksude** kui ka muude konventsioonide abil eraldi jaotisi.</span><span class="sxs-lookup"><span data-stu-id="fd9ec-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="fd9ec-115">Järgmiseks täitke jaotise "alkeemia Rule" (klientide ülevaated) jaotises Kliendi ülevaated olevate funktsioonide teksti kehatekst.</span><span class="sxs-lookup"><span data-stu-id="fd9ec-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="fd9ec-116">Täpploendid on head</span><span class="sxs-lookup"><span data-stu-id="fd9ec-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="fd9ec-117">Nummerdatud loendid on liiga</span><span class="sxs-lookup"><span data-stu-id="fd9ec-117">Numbered lists too</span></span>
    1. <span data-ttu-id="fd9ec-118">**Paks** ja *kursiiv* on a-OK</span><span class="sxs-lookup"><span data-stu-id="fd9ec-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="fd9ec-119">Lingid peavad alati olema kas **"lingid veebi"/External** või **sügavad lingid kasutajaliidese elementidele**, mitte sisemistele linkidele.</span><span class="sxs-lookup"><span data-stu-id="fd9ec-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="fd9ec-120">Pildid pole praegu ametlikult toetatud, kuid see on ka tegevuskavas.</span><span class="sxs-lookup"><span data-stu-id="fd9ec-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="fd9ec-121">Ja see on tõesti juba liiga pikk.</span><span class="sxs-lookup"><span data-stu-id="fd9ec-121">And this is really already a bit too long.</span></span> <span data-ttu-id="fd9ec-122">Head tavad on umbes 400 tähemärki---------------------------------</span><span class="sxs-lookup"><span data-stu-id="fd9ec-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="fd9ec-123">Kui teie sisu on valmis, tõmmake see otse Live ' i kontorisse.</span><span class="sxs-lookup"><span data-stu-id="fd9ec-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="fd9ec-124">Seejärel avage [alkeemia partnerite portaal](https://alchemyportal.azurewebsites.net) ja sisestage failinimi väljale URL.</span><span class="sxs-lookup"><span data-stu-id="fd9ec-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 