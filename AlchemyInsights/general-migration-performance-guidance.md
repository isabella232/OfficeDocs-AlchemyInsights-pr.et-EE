---
title: Üldised migreerimise jõudluse juhised
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3179"
ms.openlocfilehash: 10a0069c41d2e5128b2592425d815364a83b730f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932475"
---
# <a name="general-migration-performance-guidance"></a><span data-ttu-id="b13c4-102">Üldised migreerimise jõudluse juhised</span><span class="sxs-lookup"><span data-stu-id="b13c4-102">General migration performance guidance</span></span>

<span data-ttu-id="b13c4-103">**Tähtis**! Paljud SharePoint Online’i ja OneDrive’i kliendid käitavad ettevõtte jaoks olulise tähtsusega rakendusi taustal töötava teenuse suhtes.</span><span class="sxs-lookup"><span data-stu-id="b13c4-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="b13c4-104">Nende hulka kuuluvad sisu migreerimine, andmelekketõkestus (DLP) ja varunduslahendused.</span><span class="sxs-lookup"><span data-stu-id="b13c4-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="b13c4-105">Praegusel ootamatul ajal teeme kõik selleks, et SharePoint Online’i ja OneDrive’i teenused jääksid püsivalt kättesaadavaks ja töökindlaks kasutajate jaoks, kes sõltuvad kaugtööd tehes teenusest rohkem kui kunagi varem.</span><span class="sxs-lookup"><span data-stu-id="b13c4-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="b13c4-106">Selle eesmärgi toetamiseks oleme taustrakenduste (migreerimine, DLP ja varunduslahendused) jaoks rakendanud tööpäevadel päevaseks ajaks rangemad ahendamispiirangud.</span><span class="sxs-lookup"><span data-stu-id="b13c4-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="b13c4-107">Eeldatavasti on nendel rakendustel praegusel ajal väga piiratud läbilaskevõime.</span><span class="sxs-lookup"><span data-stu-id="b13c4-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="b13c4-108">Aga regiooni õhtustel aegadel ja nädalavahetustel on teenus valmis töötlema palju suuremat hulka taustrakendustest pärit taotlusi.</span><span class="sxs-lookup"><span data-stu-id="b13c4-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="b13c4-109">**Migreerimise jõudluse juhised**</span><span class="sxs-lookup"><span data-stu-id="b13c4-109">**Migration performance guidance**</span></span>

<span data-ttu-id="b13c4-110">Migreerimise jõudlust võivad mõjutada võrgutaristu, failimaht, migreerimiskellaaeg ja ahendamine.</span><span class="sxs-lookup"><span data-stu-id="b13c4-110">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling.</span></span> <span data-ttu-id="b13c4-111">Nende tegurite mõistmine aitab teil plaanida oma migreerimisprotsessi ja tagada suurim tõhusus.</span><span class="sxs-lookup"><span data-stu-id="b13c4-111">Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

- [<span data-ttu-id="b13c4-112">Üldised migreerimise jõudluse juhised</span><span class="sxs-lookup"><span data-stu-id="b13c4-112">General migration performance guidance</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
