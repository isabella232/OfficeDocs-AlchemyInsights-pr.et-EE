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
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="81b3a-102">Microsoft 365 rühma peitmine loendist aadressiloend (GAL)</span><span class="sxs-lookup"><span data-stu-id="81b3a-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="81b3a-103">Microsoft 365 rühma peitmiseks Exchange ' i klientide (nt Outlook või OWA) aadresside loenditest (nt Outlook või OWA) kasutage nuppu EKSO Shell järgmine käsk:</span><span class="sxs-lookup"><span data-stu-id="81b3a-103">To hide a Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="81b3a-104">Kui soovite, et Microsoft 365 Group peidaks end Exchange ' i klientidele nähtavana, kasutage funktsiooni EKSO Shell järgmist käsku:</span><span class="sxs-lookup"><span data-stu-id="81b3a-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

