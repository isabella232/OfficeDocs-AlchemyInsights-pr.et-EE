---
title: Majutatud kõneposti lubamine
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 4042e042554f78febff2073fde6f14db72a6d4e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318644"
---
# <a name="how-to-enable-hosted-voicemail"></a>Majutatud kõneposti lubamine

Kõneposti lubamiseks peab **HostedVoicemail** olema seatud $true.

Remote PowerShelli (RPS) abil kasutaja atribuut **HostedVoicemail (HostitudVoicemail).**

Lisateavet RPS-iga ühenduse loomise kohta [leiate teemast Microsoft Teams PowerShelli](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) ülevaade.

1. Teams administraator peaks olema sisse logitud PowerShelli kaugarvutisse Teams.
1. PowerShelli viiba kaudu Teams administraator käivitada **set-csuseri user@contoso.com -HostedVoiceMail $true** kus sip uri on selle kasutaja jaoks.

**Märkus.** Poliitikate muudatuste paljunemiseks võib aega võtta kuni 24 tundi.