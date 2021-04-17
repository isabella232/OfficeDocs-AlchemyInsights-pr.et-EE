---
title: Luba päranddialoogide kinnitamine aruannete avamiseks
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814260"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="86e4b-102">Luba päranddialoogide kinnitamine aruannete avamiseks</span><span class="sxs-lookup"><span data-stu-id="86e4b-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="86e4b-103">**Sümptom**</span><span class="sxs-lookup"><span data-stu-id="86e4b-103">**Symptom**</span></span>

<span data-ttu-id="86e4b-104">Kasutajad ei saa aruandeid avada.</span><span class="sxs-lookup"><span data-stu-id="86e4b-104">Users are unable to open reports.</span></span> <span data-ttu-id="86e4b-105">"Midagi on valesti läinud.</span><span class="sxs-lookup"><span data-stu-id="86e4b-105">"Something has gone wrong.</span></span> <span data-ttu-id="86e4b-106">Lisateabe saamiseks vaadake tehnilisi üksikasju."</span><span class="sxs-lookup"><span data-stu-id="86e4b-106">Check technical details for more details."</span></span>

<span data-ttu-id="86e4b-107">**Põhjus**</span><span class="sxs-lookup"><span data-stu-id="86e4b-107">**Cause**</span></span>

<span data-ttu-id="86e4b-108">Aruannete laadimine UCI-s nurjub tõrkega "Vormideskriptor on null või pole määratletud".</span><span class="sxs-lookup"><span data-stu-id="86e4b-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="86e4b-109">Aruanded UCI-s vajavad siiski päranddialooge, nii et kliendi süsteem peab lubama *allowlegacydialogsembedding*.</span><span class="sxs-lookup"><span data-stu-id="86e4b-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="86e4b-110">**Lahendus**</span><span class="sxs-lookup"><span data-stu-id="86e4b-110">**Solution**</span></span>

1. <span data-ttu-id="86e4b-111">Avage **Settings >Administration > System Settings > Vahekaart Üldine**.</span><span class="sxs-lookup"><span data-stu-id="86e4b-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="86e4b-112">Määrake väärtuse "Luba teatud päranddialoogide manustamine ühendatud kasutajaliidese brauserikliendis" väärtuseks **Jah**.</span><span class="sxs-lookup"><span data-stu-id="86e4b-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
