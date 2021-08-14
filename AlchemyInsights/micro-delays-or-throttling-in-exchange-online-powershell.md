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
ms.openlocfilehash: cb97aa790264c23aae15fed49c353c7fb0d6209d9492c6881f1b1091fe80d7b8
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57868530"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikro viivitused või ahendamine Exchange Online PowerShellis

Exchange Online’is skriptide ja cmdlet-käskude käitamisel võite näha hoiatusi „Mikro viivitus rakendatud“ või viivitusi. Siin on mõned soovitused selle lahendamiseks.

- Rentniku PowerShelli ahendamise poliitikate leevendamiseks käivitage meie diagnostika. See lahendus lahendab probleemi kõige rohkem.
- Kui probleem ei lahene, kasutage [Exchange Online v2 PowerShelli](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)moodulit, mis sisaldab REST API-l põhinevaid CMDlets'i ja on oluliselt rohkem esinejad. See võib olla suurepärane lahendus paljudele cmdleti hankimise käskude, mida sageli kasutatakse.
- Kui teil on vaja kasutada CMDletsi, mida v2 moodul ei hõlma, lugege teemat [PowerShelli](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)cmdlet-käskude käitamine suure hulga kasutajate jaoks Office 365-s, mis räägib powerShelli ahendamise piirangutest Exchange Online.
