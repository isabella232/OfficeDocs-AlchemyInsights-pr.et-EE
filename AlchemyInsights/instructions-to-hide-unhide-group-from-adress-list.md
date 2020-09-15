---
title: Juhised rühma peitmiseks/peitmiseks loendist aadressiloend
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 1ad9ab294d46ca0fc88a454e3503ddcf80398896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663005"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Microsoft 365 rühma peitmine loendist aadressiloend (GAL)

Microsoft 365 rühma peitmiseks Exchange ' i klientide (nt Outlook või OWA) aadresside loenditest (nt Outlook või OWA) kasutage nuppu EKSO Shell järgmine käsk:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Kui soovite, et Microsoft 365 Group peidaks end Exchange ' i klientidele nähtavana, kasutage funktsiooni EKSO Shell järgmist käsku:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

