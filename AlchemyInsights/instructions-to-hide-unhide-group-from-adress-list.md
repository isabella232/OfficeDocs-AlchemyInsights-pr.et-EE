---
title: Juhised rühma peitmiseks/peitmiseks aadressiloendis
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 61ba34e6d554831da712a92401f26fabb02c26b7
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908340"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Peida Microsoft 365 rühma aadressiloend (GAL)

Microsoft 365 rühma peitmiseks aadressiloendid (GAL) Exchange ' i klientide (nt Outlook või OWA), kasutage järgmist käsku EXO kest:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Microsoft 365 rühma peitmiseks Exchange ' i klientidele nähtavaks, kasutage järgmist käsku EXO kest:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

