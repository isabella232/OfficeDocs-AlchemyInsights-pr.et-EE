---
title: 1490 – tõrkeotsing – e-juurdlus – tõrked
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277820"
---
# <a name="troubleshoot-content-search-errors"></a><span data-ttu-id="632e4-102">Sisu otsimise tõrgete tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="632e4-102">Troubleshoot Content Search errors</span></span>

<span data-ttu-id="632e4-103">Kas teil on otsingutulemite eksportimisel probleeme sisu otsimise või nurjumisega?</span><span class="sxs-lookup"><span data-stu-id="632e4-103">Are you experiencing problems with Content Search or getting failures when you export search results?</span></span>

<span data-ttu-id="632e4-104">Kas olete näiteks saanud otsingute käitamisel järgmisi?</span><span class="sxs-lookup"><span data-stu-id="632e4-104">For example, are you receiving the following when running searches?</span></span>

- <span data-ttu-id="632e4-105">CS008 või CS012 tõrked</span><span class="sxs-lookup"><span data-stu-id="632e4-105">CS008 or CS012 errors</span></span>

- <span data-ttu-id="632e4-106">Serveri hõivatud/ajalõpu tõrked</span><span class="sxs-lookup"><span data-stu-id="632e4-106">Server busy/timeout errors</span></span>

- <span data-ttu-id="632e4-107">Rakenduse tõrge ilmnes</span><span class="sxs-lookup"><span data-stu-id="632e4-107">Application error occurred</span></span>

<span data-ttu-id="632e4-108">Või kui otsite või ekspordite tulemid suurest arvust postkastidest (üle 100 000 postkasti), saate te eksportida tõrkeid?</span><span class="sxs-lookup"><span data-stu-id="632e4-108">Or when searching or exporting results from a large number of mailboxes (over 100,000 mailboxes), are you getting export errors?</span></span>

<span data-ttu-id="632e4-109">Seda tüüpi tõrgete korral proovi uuesti otsida sisulisi asukohti, mis on nurjunud.</span><span class="sxs-lookup"><span data-stu-id="632e4-109">For these types of errors, retry the search for the content locations that have failed.</span></span> <span data-ttu-id="632e4-110">Lisateavet leiate  [sellest artiklist](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="632e4-110">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

<span data-ttu-id="632e4-111">Kui ekspordite rohkem kui 100K postkaste, peate eksportimise tulemite allalaadimiseks kasutama järgmist PowerShelli, et eksportida  [tulemid enam kui 100k postkastist](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="632e4-111">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>
