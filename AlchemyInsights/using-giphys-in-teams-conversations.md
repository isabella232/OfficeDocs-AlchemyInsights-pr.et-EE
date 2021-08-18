---
title: Giphys'i kasutamine Teams vestlustes
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
ms.openlocfilehash: 296c2f80d35f1c93ab3c60e0be65fd96c953ca81
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323516"
---
# <a name="using-giphys-in-teams-conversations"></a>Giphys'i kasutamine Teams vestlustes

Giphys access in Teams chat on vaikimisi lubatud. Administraatorina saate kontrollida, kas Giphys on [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) kasutajatele saadaval, määrates sõnumsidepoliitika ja tagades, et **Giphys'i kasutamine vestlustes** on **sees.**

Kui GIF-id ei tööta Teams ootuspäraselt, kontrollige järgmist.

[Sõnumsidepoliitika peab](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) Giphys'e lubama. PowerShelli cmdlet-käskude abil kinnitamiseks:

- Veenduge, et [powerShelli abil Teams hallata.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)
- Käivitage PowerShelli käsk [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) ja veenduge, **et AllowGiphy** väärtuseks oleks **seatud TRUE.**
- Kui **AllowGiphy väärtuseks** on **seatud FALSE,** käivitage järgmine PowerShelli käsk [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Giphy](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) URL-ile juurdepääsu võimaldamiseks peavad olema lubatud valikulised ühendatud funktsioonid.

**Märkus.** Kui teie rentniku jaoks Teams mitu Teams sõnumsidepoliitikat, saate määrata mõjutatud kasutajale määratud poliitika identiteedi PowerShelli käsu [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Valige TeamsMessagingPolicy(TeamsMessagingPolicy).
