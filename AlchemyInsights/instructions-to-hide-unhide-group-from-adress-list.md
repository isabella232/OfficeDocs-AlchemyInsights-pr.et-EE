---
title: Juhised rühma peitmiseks/peidust välja peidemiseks aadressiloendist
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 4d55866700b9b8494f1f692cd3b865116b96a1bc
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831874"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Microsoft 365 rühma peitmine aadressiloendist (GAL)

Microsoft 365 rühma peitmiseks Exchange'i klientide aadressiloendite (nt Outlooki või OWA) aadressiloendite (nt Outlooki või OWA) eest kasutage EXO shellis järgmist käsku.

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Microsoft 365 rühma Exchange'i klientklientidele nähtavaks vaatamiseks kasutage EXO kestas järgmist käsku.

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

