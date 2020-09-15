---
title: Kaasaegne sait juure saidina
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666866"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="76424-102">Kaasaegne sait juure saidina</span><span class="sxs-lookup"><span data-stu-id="76424-102">Modern site as root site</span></span>

<span data-ttu-id="76424-103">Oleme alustanud uue funktsiooni väljatöötamist, mis võimaldab teil [vahetada oma klassikalist saidi juurt modernse](https://docs.microsoft.com/sharepoint/modern-root-site)saidiga.</span><span class="sxs-lookup"><span data-stu-id="76424-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="76424-104">Kasutage [SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) , et vahetada saidi asukoht teise saidiga, arhiivides algse saidi.</span><span class="sxs-lookup"><span data-stu-id="76424-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="76424-105">Saadaval nii meeskonnatöö saidi jaoks (pole rühmaga ühendatud) kui ka kommunikatsiooni saidil.</span><span class="sxs-lookup"><span data-stu-id="76424-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="76424-106">Ärge kustutage oma klassikalist juurt, et luua kaasaegne kommunikatsiooni sait.</span><span class="sxs-lookup"><span data-stu-id="76424-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="76424-107">Microsoft ei toeta seda.</span><span class="sxs-lookup"><span data-stu-id="76424-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="76424-108">Juurte saidi kustutamine muudab kõik teie organisatsioonis olevad SharePointi saidid kõigile kasutajatele juurdepääsetavaks, kuni taastate saidi või loote sama URL-is uue saidi.</span><span class="sxs-lookup"><span data-stu-id="76424-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="76424-109">Edastame selle funktsiooni teateriba kaudu.</span><span class="sxs-lookup"><span data-stu-id="76424-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="76424-110">Peate eeldama, et funktsioon on rentniku jaoks peagi sisse lülitatud.</span><span class="sxs-lookup"><span data-stu-id="76424-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="76424-111">Saidid vahetamise teadaolevad probleemid</span><span class="sxs-lookup"><span data-stu-id="76424-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="76424-112">Sihtkaust võib tagastada lühikese aja jooksul tõrketeate "ei leitud" (HTTP 404).</span><span class="sxs-lookup"><span data-stu-id="76424-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="76424-113">Otsingu indeksi värskendamiseks tuleb sisu uuesti analüüsida.</span><span class="sxs-lookup"><span data-stu-id="76424-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="76424-114">Siin pole käsitsi vajalikku juhiseid, seda tehakse automaatselt.</span><span class="sxs-lookup"><span data-stu-id="76424-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="76424-115">Midagi, mis sõltub staatilisest lingist (nt failide sünkroonimine ja OneNote ' i failid), tuleb käsitsi parandada.</span><span class="sxs-lookup"><span data-stu-id="76424-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="76424-116">Võimalik, et Project Serveri saidid peavad olema valideeritud, et veenduda, et need on endiselt õigesti seotud.</span><span class="sxs-lookup"><span data-stu-id="76424-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
