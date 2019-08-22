---
title: Vaheta klassikaline juursait mis kaasaegne veebilehekülg
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: ffb1466fe436d6cab7ae5fdd60c671f5dd2654dd
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36501075"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="4c9c5-102">Vaheta klassikaline juursait mis kaasaegne veebilehekülg</span><span class="sxs-lookup"><span data-stu-id="4c9c5-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="4c9c5-103">Kui teie keskkonnas oli enne aprilli 2019, saate muuta oma juursait kaasaegne veebilehekülg Microsoft PowerShelli abil:</span><span class="sxs-lookup"><span data-stu-id="4c9c5-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="4c9c5-104">Kui teil on mõni muu sait, mida soovite kasutada oma juursait, saate asendada (swap) juur saidi see.</span><span class="sxs-lookup"><span data-stu-id="4c9c5-104">If you have a different site that you want to use as your root site, you can replace (swap) the root site with it.</span></span> 
    - <span data-ttu-id="4c9c5-105">Vahetada asukoht teise saidiga algse saidi arhiveerimise ajal kasutada [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="4c9c5-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="4c9c5-106">Saadaval Team Site (ühendatud rühma) ja teatise ala.</span><span class="sxs-lookup"><span data-stu-id="4c9c5-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="4c9c5-107">Võetakse kasutusele täiendavad võimalused kiiresti, mis lubab kasutada saidi sisu, kuid muuta olemasoleva saidi teatis saidile.</span><span class="sxs-lookup"><span data-stu-id="4c9c5-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="4c9c5-108">Need võimed on rullitakse järk-järgult.</span><span class="sxs-lookup"><span data-stu-id="4c9c5-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="4c9c5-109">Edasi kontrollige värskendusi Office 365 sõnumikeskus.</span><span class="sxs-lookup"><span data-stu-id="4c9c5-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="4c9c5-110">Tuntud probleemid tootega vahetada saidid</span><span class="sxs-lookup"><span data-stu-id="4c9c5-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="4c9c5-111">Sihtsaidi tagastab "ei leitud" viga (HTTP 404) lühikest aega.</span><span class="sxs-lookup"><span data-stu-id="4c9c5-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="4c9c5-112">Sisu tuleb analüüsitakse uuesti värskendada otsinguregistrisse.</span><span class="sxs-lookup"><span data-stu-id="4c9c5-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="4c9c5-113">Ei ole vaja käsitsi sammu - seda tehakse automaatselt.</span><span class="sxs-lookup"><span data-stu-id="4c9c5-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="4c9c5-114">Midagi sõltub "staatiline" lingid (nt faili sünkroonimine ja OneNote) pead käsitsi korrigeerida.</span><span class="sxs-lookup"><span data-stu-id="4c9c5-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="4c9c5-115">Kui allika ala oli organisatsiooni uudistesaidi, muudetud URL.</span><span class="sxs-lookup"><span data-stu-id="4c9c5-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="4c9c5-116">Saada kõik organisatsiooni Uudised kohad.</span><span class="sxs-lookup"><span data-stu-id="4c9c5-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="4c9c5-117">Project Serveri saidid võib tekkida vajadus tagada, et need on ikka seotud õigesti kinnitada.</span><span class="sxs-lookup"><span data-stu-id="4c9c5-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





