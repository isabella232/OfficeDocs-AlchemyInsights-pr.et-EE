---
title: NDI tehnoloogia sisselülitamine
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004403"
- "7947"
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935099"
---
# <a name="turn-on-ndi-technology"></a><span data-ttu-id="c8670-102">NDI tehnoloogia sisselülitamine</span><span class="sxs-lookup"><span data-stu-id="c8670-102">Turn on NDI technology</span></span>

<span data-ttu-id="c8670-103">NDI tehnoloogia peab kasutaja jaoks sisse lülitama kaks toimingut.</span><span class="sxs-lookup"><span data-stu-id="c8670-103">NDI technology requires two steps to be turned on for a user:</span></span>

1. <span data-ttu-id="c8670-104">Rentniku administraator peab lubama atribuudi "AllowNDIStreaming" CsTeamsMeetingPolicy.</span><span class="sxs-lookup"><span data-stu-id="c8670-104">The tenant admin must enable the 'AllowNDIStreaming' property in CsTeamsMeetingPolicy.</span></span>

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. <span data-ttu-id="c8670-105">Pärast seda, kui see muudatus on asustatud, peab lõppkasutaja NDI® tehnoloogiale oma konkreetse kliendi jaoks **> õigustest sätetest** välja lülitama.</span><span class="sxs-lookup"><span data-stu-id="c8670-105">After this change has populated, the end user must turn on NDI® technology for their specific client from **Settings > Permissions**.</span></span>

<span data-ttu-id="c8670-106">Lisateavet leiate teemast [Microsoft teamsi NDI tehnoloogia kasutamine](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).</span><span class="sxs-lookup"><span data-stu-id="c8670-106">For more information, see [Use NDI technology in Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).</span></span>
