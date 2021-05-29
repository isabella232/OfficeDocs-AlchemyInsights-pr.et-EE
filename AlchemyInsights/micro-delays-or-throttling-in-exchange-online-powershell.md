---
title: Mikro viivitused või ahendamine Exchange Online PowerShellis
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
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702122"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikro viivitused või ahendamine Exchange Online PowerShellis

Exchange Online’is skriptide ja cmdlet-käskude käitamisel võite näha hoiatusi „Mikro viivitus rakendatud“ või viivitusi. Siin on mõned soovitused selle lahendamiseks.

- Rentniku PowerShelli ahendamise poliitikate leevendamiseks käivitage meie diagnostika. See lahendus lahendab probleemi kõige rohkem.
- Kui probleem ei lahene, kasutage [Exchange Online v2 PowerShelli](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)moodulit, mis sisaldab REST API-l põhinevaid CMDlets'i ja on oluliselt rohkem esinejad. See võib olla suurepärane lahendus paljudele cmdleti hankimise käskude, mida sageli kasutatakse.
- Kui teil on vaja kasutada CMDlets'i, mida v2 moodul ei hõlma, lugege teemat [PowerShelli](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)cmdlet-käskude käitamine suure hulga kasutajate jaoks Office 365-s, mis räägib powerShelli ahendamise piirangutest Exchange Online.
