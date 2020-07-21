---
title: Kasutaja saab tõrke AADSTS7000112 Yammer on keelatud
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197872"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>Kasutaja saab tõrke AADSTS7000112 Yammer on keelatud

Kui kuvatakse tõrketeade "AADSTS7000112: rakendus '00000005-0000-0ff1-ce00-0000000000000"(Yammer) on keelatud", on probleem teenuse peamine Azure AD.-s. Administraator võib olla keelanud teenuse subjekti Yammerile juurdepääsu blokeerimiseks.

Teenuse subjekti keelamine pole soovitatav ja võib põhjustada lisaprobleeme. Lisateavet toetatud lähenemisviisi kohta, et blokeerida kasutajate juurdepääs Yammerile, leiate teemast [Yammeri juurdepääsu väljalülitamine Microsoft 365 kasutajatele](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).  

Azure'i portaali sprobleemi lahendamiseks ja yammerile kasutaja juurdepääsu taastamiseks

1.  Avage leht Azure Active Directory ja valige vasakpoolsel navigeerimispaanil jaotises **Halda** suvand **Ettevõtte rakendused.**
3.  Tippige otsinguväljale **Tekst Office 365 Yammer** ja valige sätete avamiseks rakenduse nimi.
4.  Valige vasakpoolsel navigeerimispaanil jaotises **Halda** **suvand Atribuudid.**
5.  Määrake suvandi **Lubatud kasutajatele sisselogimiseks väärtuseks** **Jah**ja seejärel valige **Salvesta**.
6.  Logige uuesti Yammerisse sisse. Võimalik, et peate küpsised kustutama.

Teise võimalusena käivitage PowerShelli käske väärtuse seadmiseks. Lisateavet leiate teemast ["Kahju, kuid meil on probleeme sisselogimisega" tõrge, kui klõpsate Office 365 paani Yammer](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365). 