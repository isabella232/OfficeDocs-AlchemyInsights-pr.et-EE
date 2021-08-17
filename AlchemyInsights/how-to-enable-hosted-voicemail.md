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
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055550"
---
# <a name="how-to-enable-hosted-voicemail"></a>Majutatud kõneposti lubamine

Kõneposti lubamiseks peab **HostedVoicemail** olema seatud $true.

Remote PowerShelli (RPS) abil kasutaja atribuut **HostedVoicemail (HostitudVoicemail).**

Lisateavet RPS-iga ühenduse loomise kohta [leiate teemast Microsoft Teams PowerShelli](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) ülevaade.

1. Administraator Teams logitakse PowerShelli kaugarvutisse Teams.
1. PowerShelli viiba kaudu Teams administraator käivitada **set-csuseri user@contoso.com -HostedVoiceMail $true** kus sip uri on kõnealuse kasutaja jaoks.

> [!NOTE]
> Poliitikate muudatuste paljunemiseks võib aega võtta kuni 24 tundi.