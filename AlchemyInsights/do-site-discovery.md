---
title: Saidi tuvastamine
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692935"
---
# <a name="do-site-discovery"></a><span data-ttu-id="52976-102">Saidi tuvastamine</span><span class="sxs-lookup"><span data-stu-id="52976-102">Do site discovery</span></span>

<span data-ttu-id="52976-103">Kui teie ettevõte kasutab endiselt pärandist veebirakendusi ja plaanib kasutada Internet Exploreri režiimi (mida enamik kliente ei kasuta), peaksite tegema mõne muu saidi tuvastamise.</span><span class="sxs-lookup"><span data-stu-id="52976-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="52976-104">**Olete juba juurutanud Microsoft Edge ' i varasema versiooni**</span><span class="sxs-lookup"><span data-stu-id="52976-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="52976-105">Kui olete oma ettevõtte saidi loendi juba konfigureerinud töötama Microsoft Edge ' i Legacy-versioonis, on teie saidi tuvastus peaaegu valmis.</span><span class="sxs-lookup"><span data-stu-id="52976-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="52976-106">Võimalik, et peate lisama neutraalseid saite.</span><span class="sxs-lookup"><span data-stu-id="52976-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="52976-107">Neutraalsed saidid on tavaliselt saidid, mis pakuvad ühekordse sisselogimise (SSO).</span><span class="sxs-lookup"><span data-stu-id="52976-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="52976-108">Kui lähete Microsoft Edge ' i neutraalsele saidile, soovite autentida Microsoft Edge ' i.</span><span class="sxs-lookup"><span data-stu-id="52976-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="52976-109">Kui lähete Internet Exploreri režiimis neutraalsele saidile, siis soovite autentida Internet Exploreri režiimis.</span><span class="sxs-lookup"><span data-stu-id="52976-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="52976-110">Tuvastage kõik SSO või muud neutraalsed saidid, mida kasutate, ja lisage need oma ettevõtte saidi loendisse.</span><span class="sxs-lookup"><span data-stu-id="52976-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="52976-111">**Internet Explorer on teie vaikebrauser**</span><span class="sxs-lookup"><span data-stu-id="52976-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="52976-112">Kui kasutate praegu ainult Internet Explorerit, ei pruugi te teada saada, millised saidid on täiendatud moodsate veebistandarditega ja mis vajavad endiselt Internet Explorerit.</span><span class="sxs-lookup"><span data-stu-id="52976-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="52976-113">Te soovite leida ja lisada need saidid ettevõtte saidi loendisse, et saaksite kasutada Internet Exploreri režiimi ainult nende saitide jaoks.</span><span class="sxs-lookup"><span data-stu-id="52976-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="52976-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) avastab saidid, mis võivad vajada Internet Exploreri režiimi.</span><span class="sxs-lookup"><span data-stu-id="52976-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="52976-115">See võib koguda andmeid arvutites, kus töötab Windows Internet Explorer 8 Internet Explorer 11 kaudu opsüsteemis Windows 10, Windows 8,1 või Windows 7.</span><span class="sxs-lookup"><span data-stu-id="52976-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="52976-116">**Andmete analüüsimine**</span><span class="sxs-lookup"><span data-stu-id="52976-116">**Analyze the data**</span></span>

<span data-ttu-id="52976-117">Kui olete saidi andmed kogunud, soovitame andmete analüüsimiseks järgmisi nelja-etapilisi toiminguid.</span><span class="sxs-lookup"><span data-stu-id="52976-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="52976-118">Sortige andmed domeeni järgi ja seejärel URL-i järgi.</span><span class="sxs-lookup"><span data-stu-id="52976-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="52976-119">Saate määratleda Internet Exploreri režiimi konfigureerimiseks kasutatava rakenduse piirid.</span><span class="sxs-lookup"><span data-stu-id="52976-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="52976-120">Soovite kaasata kõik rakenduse määratlevad saidid ja veebihaldused, kuid te ei soovi lisada täiendavaid saite ja juhtelemente.</span><span class="sxs-lookup"><span data-stu-id="52976-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="52976-121">Mõned saidid võivad olla nii lihtsad, kui *https://contoso.com/app1* teised võivad nõuda mitme saidi ja lehe määratlemist.</span><span class="sxs-lookup"><span data-stu-id="52976-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="52976-122">Testige rakendust, et veenduda, et see ei tööta algupäraselt.</span><span class="sxs-lookup"><span data-stu-id="52976-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="52976-123">Paljud saidid pakuvad moodsat brauserit, kui nad avastavad modernse brauseri ja pakuvad Internet Exploreri tuvastamisel ainult pärandist sisu.</span><span class="sxs-lookup"><span data-stu-id="52976-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="52976-124">Lisage rakendus oma ettevõtte saidi loendisse, kui test nurjub.</span><span class="sxs-lookup"><span data-stu-id="52976-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="52976-125">Parima tavana rühmitage kõik saidid, mis moodustavad rakenduse.</span><span class="sxs-lookup"><span data-stu-id="52976-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="52976-126">Nii on rakenduse täiendamisel hõlpsam eemaldada kogu sait Internet Exploreri režiimist ja alustada selle rakenduse jaoks moodsate brauserite kasutamist.</span><span class="sxs-lookup"><span data-stu-id="52976-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="52976-127">Kui olete saidi tuvastamisega lõpetanud ja olete andmed analüüsinud, olete valmis alustama oma kanali strateegiat.</span><span class="sxs-lookup"><span data-stu-id="52976-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

