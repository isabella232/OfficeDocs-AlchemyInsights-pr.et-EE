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
ms.openlocfilehash: 6753dcb375ea5e19b01c4350b61aa8904aa102112df175a3f70281d18a634dbf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098562"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikro viivitused või ahendamine Exchange Online PowerShellis

Exchange Online’is skriptide ja cmdlet-käskude käitamisel võite näha hoiatusi „Mikro viivitus rakendatud“ või viivitusi. Siin on mõned soovitused selle lahendamiseks.

- Rentniku PowerShelli ahendamise poliitikate leevendamiseks käivitage meie diagnostika. See lahendus lahendab probleemi kõige rohkem.
- Kui probleem ei lahene, kasutage [Exchange Online v2 PowerShelli](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)moodulit, mis sisaldab REST API-l põhinevaid CMDlets'i ja on oluliselt rohkem esinejad. See võib olla suurepärane lahendus paljudele cmdleti hankimise käskude, mida sageli kasutatakse.
- Kui teil on vaja kasutada CMDlets'i, mida v2 moodul ei hõlma, lugege teemat [PowerShelli](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)cmdlet-käskude käitamine suure hulga kasutajate jaoks Office 365-s, mis räägib powerShelli ahendamise piirangutest Exchange Online.
