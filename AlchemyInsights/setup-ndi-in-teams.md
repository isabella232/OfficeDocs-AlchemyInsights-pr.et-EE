---
title: NDI-tehnoloogia sisselülitamine
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
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023518"
---
# <a name="turn-on-ndi-technology"></a>NDI-tehnoloogia sisselülitamine

NDI-tehnoloogia kasutamiseks peab kasutaja jaoks olema sisse lülitatud kaks etappi.

1. Rentnikuadministraator peab CsTeamsMeetingPolicys lubama atribuudi "AllowNDIStreaming".

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Kui see muudatus on asustatud, peab lõppkasutaja NDI® oma konkreetse kliendi jaoks sisse lülitama **Sätted > õigused**.

Lisateavet leiate teemast [NDI tehnoloogia kasutamine Microsoft Teams.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)
