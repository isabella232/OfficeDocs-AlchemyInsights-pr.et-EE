---
title: Hostitud kõneposti lubamise lubamine
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
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677334"
---
# <a name="how-to-enable-hosted-voicemail"></a>Hostitud kõneposti lubamise lubamine

Kõneposti lubamiseks peab **HostedVoicemail** olema seatud $TRUE.

Kasutaja **HostedVoicemail** atribuut Remote POWERSHELL (RPS) abil.

Lisateavet RPS-ga ühenduse loomise kohta leiate teemast [Microsoft teamsi PowerShelli ülevaade](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) RPS-ga ühenduse loomise kohta.

1. Teamsi administraator peaks olema teamsi jaoks sisse logitud Remote PowerShell.
1. PowerShelli viibal saab Teamsi administraator käitada **Set-csuser User@contoso.com-HostedVoiceMail $True** , kus on valitud kasutaja SIP-i URI.

> [!NOTE]
> Poliitikate muudatused võivad paljunemiseks kuluda kuni 24 tundi.