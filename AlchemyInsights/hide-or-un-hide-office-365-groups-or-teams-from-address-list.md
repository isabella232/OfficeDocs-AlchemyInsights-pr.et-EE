---
title: Office 365 rühmade või töörühmade peitmine või peitmine aadressiloendist
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
- "9002947"
- "5642"
ms.openlocfilehash: 12e221c69775f3dfeed1781b70d3061e1ca0ac3b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811452"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a><span data-ttu-id="6cee7-102">Office 365 rühmade või töörühmade peitmine või peitmine aadressiloendist</span><span class="sxs-lookup"><span data-stu-id="6cee7-102">Hide or un-hide Office 365 groups or teams from address list</span></span>

<span data-ttu-id="6cee7-103">Office 365 rühma/töörühmade peitmiseks või peitmiseks Exchange'i klientklientide aadressiloenditest (GAL) (Outlook, OWA) kasutage järgmist EXO PowerShelli käsku.</span><span class="sxs-lookup"><span data-stu-id="6cee7-103">Use the following EXO PowerShell command to hide or un-hide Office 365 group/teams from address lists (GAL) of Exchange clients (Outlook, OWA):</span></span>

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

<span data-ttu-id="6cee7-104">Office365 rühma/töörühmade peitmiseks või peitmiseks Exchange'i klientklientidest (Outlook, OWA) kasutage järgmist EXO PowerShelli käsku.</span><span class="sxs-lookup"><span data-stu-id="6cee7-104">Use the following EXO PowerShell command to hide or un-hide the Office365 group/teams from Exchange clients (Outlook, OWA):</span></span>

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- <span data-ttu-id="6cee7-105">Üksikasjalikud juhised leiate teemast [Office 365 rühmade peitmine GAL-i ja Exchange'i klientklientide eest.](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)</span><span class="sxs-lookup"><span data-stu-id="6cee7-105">For detailed instructions, see [Hide Office 365 Groups from the GAL and Exchange Clients](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).</span></span>
