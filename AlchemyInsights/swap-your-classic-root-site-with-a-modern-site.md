---
title: Vaheta oma Classic root saidi kaasaegne sait
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741540"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="b9e20-102">Vaheta oma Classic root saidi kaasaegne sait</span><span class="sxs-lookup"><span data-stu-id="b9e20-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="b9e20-103">Kui teie keskkond on seadistatud enne aprill 2019, saate muuta oma juursaiti kaasaegne sait, kasutades Microsoft PowerShelli:</span><span class="sxs-lookup"><span data-stu-id="b9e20-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="b9e20-104">Kui teil on erinev sait, mida soovite kasutada oma root saidi, saate asendada [(swap) root saidi](https://docs.microsoft.com/sharepoint/modern-root-site) koos sellega.</span><span class="sxs-lookup"><span data-stu-id="b9e20-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="b9e20-105">Kasutage [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) vahetada saidi asukoha teise saidi arhiveerimise algse saidi.</span><span class="sxs-lookup"><span data-stu-id="b9e20-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="b9e20-106">Saadaval nii meeskonnatöö sait (ei ole ühendatud rühma) ja side saidi.</span><span class="sxs-lookup"><span data-stu-id="b9e20-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="b9e20-107">Varsti võetakse kasutusele täiendavad võimalused, mis võimaldavad teil saidi sisu kasutada, kuid teisendage olemasolev sait suhtlussaidile.</span><span class="sxs-lookup"><span data-stu-id="b9e20-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="b9e20-108">Need võimed tehakse järk-järgult.</span><span class="sxs-lookup"><span data-stu-id="b9e20-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="b9e20-109">Jätkake teadete keskuse värskenduste kontrollimiseks.</span><span class="sxs-lookup"><span data-stu-id="b9e20-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="b9e20-110">Teadaolevad probleemid vahetamise saidid</span><span class="sxs-lookup"><span data-stu-id="b9e20-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="b9e20-111">Target sait võib tagastada "ei leitud" (HTTP 404) tõrge lühikese aja jooksul.</span><span class="sxs-lookup"><span data-stu-id="b9e20-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="b9e20-112">Otsinguindeksi värskendamiseks tuleb sisu uuesti värskendada.</span><span class="sxs-lookup"><span data-stu-id="b9e20-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="b9e20-113">Ei ole manuaalset sammu vaja-seda tehakse automaatselt.</span><span class="sxs-lookup"><span data-stu-id="b9e20-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="b9e20-114">Midagi sõltub "staatiline" linke (nt faili sünkroonimine ja OneNote faile) tuleb käsitsi parandada.</span><span class="sxs-lookup"><span data-stu-id="b9e20-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="b9e20-115">Kui Lähtesait oli organisatsiooni uudistesait, värskendage URL-i.</span><span class="sxs-lookup"><span data-stu-id="b9e20-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="b9e20-116">Saate hankida kõigi organisatsiooniuudiste saitide loendi.</span><span class="sxs-lookup"><span data-stu-id="b9e20-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="b9e20-117">Project Serveri saidid võib olla vaja valideerida, et tagada, et need on endiselt õigesti seotud.</span><span class="sxs-lookup"><span data-stu-id="b9e20-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
