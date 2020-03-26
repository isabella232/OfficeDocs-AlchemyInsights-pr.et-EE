---
title: Migreerimishalduri kaudu SharePoint Online’i migreerimine
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
- "3192"
ms.openlocfilehash: 5aebf7903670e74f616c8f151749d760caf1d642
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931972"
---
# <a name="migrating-to-sharepoint-online-via-migration-manager"></a><span data-ttu-id="db3f9-102">Migreerimishalduri kaudu SharePoint Online’i migreerimine</span><span class="sxs-lookup"><span data-stu-id="db3f9-102">Migrating to SharePoint Online via Migration Manager</span></span>

<span data-ttu-id="db3f9-103">**Tähtis**! Paljud SharePoint Online’i ja OneDrive’i kliendid käitavad ettevõtte jaoks olulise tähtsusega rakendusi taustal töötava teenuse suhtes.</span><span class="sxs-lookup"><span data-stu-id="db3f9-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="db3f9-104">Nende hulka kuuluvad sisu migreerimine, andmelekketõkestus (DLP) ja varunduslahendused.</span><span class="sxs-lookup"><span data-stu-id="db3f9-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="db3f9-105">Praegusel ootamatul ajal teeme kõik selleks, et SharePoint Online’i ja OneDrive’i teenused jääksid püsivalt kättesaadavaks ja töökindlaks kasutajate jaoks, kes sõltuvad kaugtööd tehes teenusest rohkem kui kunagi varem.</span><span class="sxs-lookup"><span data-stu-id="db3f9-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="db3f9-106">Selle eesmärgi toetamiseks oleme taustrakenduste (migreerimine, DLP ja varunduslahendused) jaoks rakendanud tööpäevadel päevaseks ajaks rangemad ahendamispiirangud.</span><span class="sxs-lookup"><span data-stu-id="db3f9-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="db3f9-107">Eeldatavasti on nendel rakendustel praegusel ajal väga piiratud läbilaskevõime.</span><span class="sxs-lookup"><span data-stu-id="db3f9-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="db3f9-108">Aga regiooni õhtustel aegadel ja nädalavahetustel on teenus valmis töötlema palju suuremat hulka taustrakendustest pärit taotlusi.</span><span class="sxs-lookup"><span data-stu-id="db3f9-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="db3f9-109">**Migreerimishaldur**</span><span class="sxs-lookup"><span data-stu-id="db3f9-109">**Migration Manager**</span></span>

<span data-ttu-id="db3f9-110">Kaasaegses SharePointi halduskeskuses asuv Migreerimishaldur juhendab teid läbi teie klientide seadistamise ja ülesannete loomise.</span><span class="sxs-lookup"><span data-stu-id="db3f9-110">Located in the modern SharePoint Admin Center, the Migration Manager guides you through the setup of your clients and the creation of your tasks.</span></span> <span data-ttu-id="db3f9-111">Saate määrata globaalsed ja ülesande tasemel seadistused, vaadata kõikehõlmavate toimingute edenemist ja laadida alla koondatud kokkuvõtte ning ülesande tasemel aruanded.</span><span class="sxs-lookup"><span data-stu-id="db3f9-111">You can specify global or task-level settings, view all-up task progress, and download aggregated summary and task-level reports.</span></span>

- [<span data-ttu-id="db3f9-112">Migreerimishalduri kasutamise alustamine</span><span class="sxs-lookup"><span data-stu-id="db3f9-112">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="db3f9-113">Migreerimishalduri klientide häälestamine</span><span class="sxs-lookup"><span data-stu-id="db3f9-113">Setup Migration Manager clients</span></span>](https://docs.microsoft.com/sharepointmigration/mm-setup-clients)

- [<span data-ttu-id="db3f9-114">Migreerimishalduri sätted</span><span class="sxs-lookup"><span data-stu-id="db3f9-114">Migration Manager Settings</span></span>](https://docs.microsoft.com/sharepointmigration/mm-settings)
