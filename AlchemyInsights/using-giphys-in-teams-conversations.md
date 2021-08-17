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
ms.openlocfilehash: 0244b68ffa2ebd3d70bae66a24ac299004848557b63b17c2ea74fafaff22bb8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104304"
---
# <a name="using-giphys-in-teams-conversations"></a>Giphys'i kasutamine Teams vestlustes

Giphys access in Teams chat on vaikimisi lubatud. Administraatorina saate kontrollida, kas Giphys on [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) kasutajatele saadaval, määrates sõnumsidepoliitika ja tagades, et **Giphys'i** kasutamine vestlustes on **sees.**

Kui GIF-id ei tööta Teams vestluses ootuspäraselt, kontrollige järgmist.

[Sõnumsidepoliitika peab](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) Giphys'e lubama. PowerShelli cmdlet-käskude abil kinnitamiseks:

- Veenduge, et [powerShelli abil Teams hallata.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)
- Käivitage PowerShelli käsk [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) ja veenduge, **et AllowGiphy** väärtuseks oleks **seatud TRUE.**
- Kui **AllowGiphy väärtuseks** on **seatud FALSE,** käivitage järgmine PowerShelli käsk [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Giphy](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) URL-ile juurdepääsu võimaldamiseks peavad olema lubatud valikulised ühendatud funktsioonid.

> [!NOTE]
> Kui teie rentniku jaoks on konfigureeritud mitu Teams sõnumsidepoliitikat, saate määratleda mõjutatud kasutajale määratud poliitika identiteedi PowerShelli [käsuga Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Valige TeamsMessagingPolicy(TeamsMessagingPolicy).
