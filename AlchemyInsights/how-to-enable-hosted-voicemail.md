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
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="cf171-102">Hostitud kõneposti lubamise lubamine</span><span class="sxs-lookup"><span data-stu-id="cf171-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="cf171-103">Kõneposti lubamiseks peab **HostedVoicemail** olema seatud $TRUE.</span><span class="sxs-lookup"><span data-stu-id="cf171-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="cf171-104">Kasutaja **HostedVoicemail** atribuut Remote POWERSHELL (RPS) abil.</span><span class="sxs-lookup"><span data-stu-id="cf171-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="cf171-105">Lisateavet RPS-ga ühenduse loomise kohta leiate teemast [Microsoft teamsi PowerShelli ülevaade](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) RPS-ga ühenduse loomise kohta.</span><span class="sxs-lookup"><span data-stu-id="cf171-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="cf171-106">Teamsi administraator peaks olema teamsi jaoks sisse logitud Remote PowerShell.</span><span class="sxs-lookup"><span data-stu-id="cf171-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="cf171-107">PowerShelli viibal saab Teamsi administraator käitada **Set-csuser User@contoso.com-HostedVoiceMail $True** , kus on valitud kasutaja SIP-i URI.</span><span class="sxs-lookup"><span data-stu-id="cf171-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="cf171-108">Poliitikate muudatused võivad paljunemiseks kuluda kuni 24 tundi.</span><span class="sxs-lookup"><span data-stu-id="cf171-108">Changes to policies can take up to 24 hours to replicate.</span></span>