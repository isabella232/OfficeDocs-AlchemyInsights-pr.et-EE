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
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Office 365 rühmade või töörühmade peitmine või peitmine aadressiloendist

Office 365 rühma/töörühmade peitmiseks või peitmiseks Exchange'i klientklientide aadressiloenditest (GAL) (Outlook, OWA) kasutage järgmist EXO PowerShelli käsku.

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Office365 rühma/töörühmade peitmiseks või peitmiseks Exchange'i klientklientidest (Outlook, OWA) kasutage järgmist EXO PowerShelli käsku.

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Üksikasjalikud juhised leiate teemast [Office 365 rühmade peitmine GAL-i ja Exchange'i klientklientide eest.](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)
