---
title: Giphy kasutamine meeskonnatöö vestlustes
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982459"
---
# <a name="using-giphys-in-teams-conversations"></a>Giphy kasutamine meeskonnatöö vestlustes

Giphy juurdepääs meeskonnatöö vestlusele on vaikimisi lubatud. Administraatorina saate määrata, kas Giphy on kasutajate jaoks saadaval, [häälestades sõnumite saatmise poliitika](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) ning tagades, et **giphy kasutamine vestlustes** on **sisse lülitatud**.

Kui gif-töö ei tööta töörühma vestlustes oodatud viisil, siis veenduge, et:

[Sõnumite poliitika](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) peab võimaldama giphy. PowerShelli cmdlet-käskude abil kinnitamiseks tehke järgmist.

- Veenduge, et saate [hallata PowerShelli abil töörühmi](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Käivitage PowerShelli käsk [Get-CsTeamsMessagingPolicy](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) ja veenduge, et **AllowGiphy** oleks seatud väärtusele **True**.
- Kui **AllowGiphy** väärtuseks on seatud **FALSE** , käivitage järgmine PowerShelli Command [Set-CsTeamsMessagingPolicy-Identity Global-AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

Giphy URL-ile juurdepääsu lubamiseks peab olema lubatud [Valikuline ühendatud kogemus](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) .

> [!NOTE]
> Kui teie rentniku jaoks on konfigureeritud mitu töörühma, saate määrata mõjutatud kasutajale määratud poliitika identiteedi, kus on PowerShelli käsk [Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Valige TeamsMessagingPolicy.
