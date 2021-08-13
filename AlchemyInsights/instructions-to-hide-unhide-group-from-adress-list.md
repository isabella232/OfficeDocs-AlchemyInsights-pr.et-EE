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
ms.openlocfilehash: af7085890d295cf0c41e11aaf18e404313413100cb8a1134bfac051d5fa26996
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926241"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Rühma Microsoft 365 peitmine aadressiloendist (GAL)

Rühma Microsoft 365 (GAL) Exchange (nt Outlook või OWA) aadressiloendite (GAL) jaoks kasutage EXO kestas järgmist käsku.

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Kui soovite, Microsoft 365 rühma ei kuvataks Exchange, kasutage EXO kestas järgmist käsku.

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

