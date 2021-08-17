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
ms.openlocfilehash: 2fab21f76f455815979ae162c1ce8246ad5c297e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314696"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikro viivitused või ahendamine Exchange Online PowerShellis

Exchange Online’is skriptide ja cmdlet-käskude käitamisel võite näha hoiatusi „Mikro viivitus rakendatud“ või viivitusi. Siin on mõned soovitused selle lahendamiseks.

- Rentniku PowerShelli ahendamise poliitikate leevendamiseks käivitage meie diagnostika. See lahendus lahendab probleemi kõige rohkem.
- Kui probleem ei lahene, kasutage [Exchange Online v2 PowerShelli](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)moodulit, mis sisaldab REST API-l põhinevaid CMDlets'i ja on oluliselt rohkem esinejad. See võib olla suurepärane lahendus paljudele cmdleti hankimise käskude, mida sageli kasutatakse.
- Kui teil on vaja kasutada CMDletsi, mida v2-moodulis ei hõlma, lugege teemat [PowerShelli](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)cmdlet-käskude käitamine suure hulga kasutajate jaoks Office 365-s, mis räägib powerShelli ahendamise piirangutest Exchange Online.
