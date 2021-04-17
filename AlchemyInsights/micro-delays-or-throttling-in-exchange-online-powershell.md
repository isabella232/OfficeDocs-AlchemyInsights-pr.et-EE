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
ms.openlocfilehash: 680df9e6e2404ff6b60b17d6ac88e202e9a7bb25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830029"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikro viivitused või ahendamine Exchange Online PowerShellis

Exchange Online’is skriptide ja cmdlet-käskude käitamisel võite näha hoiatusi „Mikro viivitus rakendatud“ või viivitusi. Järgnevalt on toodud sellega seoses kaks soovitust.

- Võite proovida kasutada [Exchange Online’i versiooni 2 PowerShelli moodulit](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), mis sisaldab cmdlet-käske, mis põhinevad REST API-l ja mida teostatakse olulised rohkem. See võib olla suurepärane lahendus paljudele cmdleti hankimise käskude, mida sageli kasutatakse.
- Kui peate kasutama cmdlet-käske, mis ei ole versiooni 2 moodulis veel kaetud, vaadake teemat [PowerShelli cmdlet-käskude käitamine paljudele Office 365 kasutajatele](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), mis selgitab, kuidas navigeerida oodatud PowerShelli ahendamise piirangutes Exchange Online’is.
