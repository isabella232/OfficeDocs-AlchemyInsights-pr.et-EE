---
title: Klassikalise saidi vahetamine moodsa saidiga
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691175"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="f8be5-102">Klassikalise saidi vahetamine moodsa saidiga</span><span class="sxs-lookup"><span data-stu-id="f8be5-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="f8be5-103">Kui teie keskkond oli häälestatud enne 2019 aprillini, saate Microsoft PowerShelli abil muuta oma juure modernseks saidiks.</span><span class="sxs-lookup"><span data-stu-id="f8be5-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="f8be5-104">Kui teil on mõni muu sait, mida soovite kasutada oma juure saidina, saate selle [saidi asendada (swap)](https://docs.microsoft.com/sharepoint/modern-root-site) .</span><span class="sxs-lookup"><span data-stu-id="f8be5-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="f8be5-105">Kasutage [SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) , et vahetada saidi asukoht teise saidiga, arhiivides algse saidi.</span><span class="sxs-lookup"><span data-stu-id="f8be5-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="f8be5-106">Saadaval nii meeskonnatöö saidi jaoks (pole rühmaga ühendatud) kui ka kommunikatsiooni saidil.</span><span class="sxs-lookup"><span data-stu-id="f8be5-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="f8be5-107">Lisavõimalused võetakse kasutusele varsti, mis võimaldab teil saidil olevat sisu kasutada, kuid olemasoleva saidi saidiks teisendada.</span><span class="sxs-lookup"><span data-stu-id="f8be5-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="f8be5-108">Need võimalused on järk-järgult rullitud.</span><span class="sxs-lookup"><span data-stu-id="f8be5-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="f8be5-109">Jätkake värskenduste otsimist.</span><span class="sxs-lookup"><span data-stu-id="f8be5-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="f8be5-110">Saidid vahetamise teadaolevad probleemid</span><span class="sxs-lookup"><span data-stu-id="f8be5-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="f8be5-111">Sihtkaust võib tagastada lühikese aja jooksul tõrketeate "ei leitud" (HTTP 404).</span><span class="sxs-lookup"><span data-stu-id="f8be5-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="f8be5-112">Otsingu indeksi värskendamiseks tuleb sisu uuesti analüüsida.</span><span class="sxs-lookup"><span data-stu-id="f8be5-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="f8be5-113">Käsitsi tehtavaid juhiseid pole vaja – seda tehakse automaatselt.</span><span class="sxs-lookup"><span data-stu-id="f8be5-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="f8be5-114">Midagi, mis sõltub staatilisest lingist (nt failide sünkroonimine ja OneNote ' i failid), tuleb käsitsi parandada.</span><span class="sxs-lookup"><span data-stu-id="f8be5-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="f8be5-115">Kui lähteteksti sait oli ettevõtte uudiste sait, värskendage URL-i.</span><span class="sxs-lookup"><span data-stu-id="f8be5-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="f8be5-116">Hankige kõigi organisatsiooniliste uudiste saitide loend.</span><span class="sxs-lookup"><span data-stu-id="f8be5-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="f8be5-117">Võimalik, et Project Serveri saidid peavad olema valideeritud, et veenduda, et need on endiselt õigesti seotud.</span><span class="sxs-lookup"><span data-stu-id="f8be5-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
