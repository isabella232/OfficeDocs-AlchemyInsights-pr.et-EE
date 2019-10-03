---
title: Poliitikasätete koosolek
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376604"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Microsoft Teamsi koosolekupoliitikate haldamine

Koosolekupoliitikaid kasutatakse nende funktsioonide juhtimiseks, mis on saadaval osavõtjatele koosolekuteks, mis on planeeritud teie organisatsiooni kasutajate poolt. Mõned koosolekupoliitikate funktsioonid ei pruugi veel meeskondi administreerimiskeskuses rakendada (need on dokumentatsioonis märgistatud "peatselt"). Sel juhul või kui saate tõrketeate, nagu "me ei saa värskendada poliitika kohe, kuid proovige seda hiljem uuesti" Microsoft Teams halduskeskus, soovitame kasutada PowerShelli luua või muuta meeskondade koosolekute poliitikad. 

Koosolekupoliitikate kohta lisateabe saamiseks vaadake järgmisi ressursse:

- Poliitikate loomise, muutuste tegemise ja poliitika kasutajate määramise kohta leiate teavet teemast [teamsi koosolekute poliitikate haldamine](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).

- Poliitika muudatuste tegemiseks PowerShelli cmdlet-käskude abil vaadake teemat [Teamsi PowerShelli ülevaade](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Peate kasutama [Skype Business PowerShelli moodul](https://www.microsoft.com/download/details.aspx?id=39366) meeskonnad koosoleku poliitika. 
    - Vaadake üle [*-csteamsmeetingpolicy cmdlet-käskude dokumentatsiooni](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) lisateabe saamiseks.

**Märkus:** Poliitika muudatuste jõustumiseks kasutajatele võib kuluda kuni 24 tundi. Võimalik, et te ei saa äsja loodud poliitikaid kohe muuta; Oodake 4 tundi ja proovige äsja loodud poliitikat uuesti muuta. Kui teil on endiselt probleeme, proovige PowerShelli.  