---
title: Kaasaegne sait kui root sait
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2e2bb02b9dbaf7f8ede0b4c5ba8c8f29453309cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054698"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="5d1d1-102">Kaasaegne sait root sait</span><span class="sxs-lookup"><span data-stu-id="5d1d1-102">Modern site as root site</span></span>

<span data-ttu-id="5d1d1-103">Oleme hakanud rollout uus funktsioon, mis võimaldab teil [vahetada oma klassikalise saidi root saidi kaasaegse saidi](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="5d1d1-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="5d1d1-104">Kasutage [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) vahetada saidi asukoha teise saidi arhiveerimise algse saidi.</span><span class="sxs-lookup"><span data-stu-id="5d1d1-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="5d1d1-105">Saadaval nii meeskonnatöö sait (ei ole ühendatud rühma) ja side saidi.</span><span class="sxs-lookup"><span data-stu-id="5d1d1-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="5d1d1-106">Ärge kustutage oma klassikalist juursaiti, et luua kaasaegne Kommunikatsioonisait.</span><span class="sxs-lookup"><span data-stu-id="5d1d1-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="5d1d1-107">Microsoft ei toeta seda.</span><span class="sxs-lookup"><span data-stu-id="5d1d1-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="5d1d1-108">Juursaidi kustutamisel tehakse kõik SharePointi saidid teie organisatsioonis kättesaamatuks kõigile kasutajatele, kuni saate saidi taastada või luua uue saidi samas URL-is.</span><span class="sxs-lookup"><span data-stu-id="5d1d1-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="5d1d1-109">Edastame selle funktsiooni sõnumikeskuse kaudu.</span><span class="sxs-lookup"><span data-stu-id="5d1d1-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="5d1d1-110">Peaksite ootama, et funktsioon oleks teie rentnikus peagi sisse lülitatud.</span><span class="sxs-lookup"><span data-stu-id="5d1d1-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="5d1d1-111">Teadaolevad probleemid vahetamise saidid</span><span class="sxs-lookup"><span data-stu-id="5d1d1-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="5d1d1-112">Target sait võib tagastada "ei leitud" (HTTP 404) tõrge lühikese aja jooksul.</span><span class="sxs-lookup"><span data-stu-id="5d1d1-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="5d1d1-113">Otsinguindeksi värskendamiseks tuleb sisu uuesti värskendada.</span><span class="sxs-lookup"><span data-stu-id="5d1d1-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="5d1d1-114">Siin ei ole manuaalset sammu vaja, seda tehakse automaatselt.</span><span class="sxs-lookup"><span data-stu-id="5d1d1-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="5d1d1-115">Midagi sõltub "staatiline" linke (nt faili sünkroonimine ja OneNote faile) tuleb käsitsi parandada.</span><span class="sxs-lookup"><span data-stu-id="5d1d1-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="5d1d1-116">Project Serveri saidid võib olla vaja valideerida, et tagada, et need on endiselt õigesti seotud.</span><span class="sxs-lookup"><span data-stu-id="5d1d1-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
