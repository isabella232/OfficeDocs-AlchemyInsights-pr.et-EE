---
title: Rühmade või töörühmade Office 365 peitmine või peitmine aadressiloendist
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
ms.openlocfilehash: 7e667e22cd81f38a1a2c1385bf42e5227cb641480f4b505110ee7349a13f13a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088392"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Rühmade või töörühmade Office 365 peitmine või peitmine aadressiloendist

Järgmiste EXO PowerShelli käskude abil saate Office 365 rühmad/meeskonnad Exchange (Outlook, OWA) aadressiloenditest.

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Office365 rühma/töörühmade peitmiseks või peitmiseks Exchange (Outlook, OWA) kasutage järgmist EXO PowerShelli käsku.

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Üksikasjalikud juhised leiate teemast [Office 365 rühmade peitmine GAL-i ja Exchange klienti](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).
