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
ms.openlocfilehash: d0e0285701f1a5f308bdc682abaddf5cc2d34120
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768914"
---
# <a name="hide-office-365-group-from-address-list-gal"></a>Peida Office 365 rühma aadressiloend (GAL)

Office 365 rühma peitmiseks aadressiloendid (GAL) Exchange ' i klientide (nt Outlook või OWA), kasutage järgmist käsku EXO kest:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Office 365 rühma peitmiseks Exchange ' i klientidele nähtavaks, kasutage järgmist käsku EXO kest:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

