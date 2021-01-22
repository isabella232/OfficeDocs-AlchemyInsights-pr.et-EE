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
# <a name="turn-on-ndi-technology"></a>NDI tehnoloogia sisselülitamine

NDI tehnoloogia peab kasutaja jaoks sisse lülitama kaks toimingut.

1. Rentniku administraator peab lubama atribuudi "AllowNDIStreaming" CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Pärast seda, kui see muudatus on asustatud, peab lõppkasutaja NDI® tehnoloogiale oma konkreetse kliendi jaoks **> õigustest sätetest** välja lülitama.

Lisateavet leiate teemast [Microsoft teamsi NDI tehnoloogia kasutamine](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).
