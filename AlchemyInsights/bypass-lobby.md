---
title: Möödu fuajee
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: bf8be9ffe2bfa45ed2cf149c1c4fa118b40e816d
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768436"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Fuajeeseadete ja osalemise taseme kontrollimine

Kui soovite lubada kõigil, sh sissehelistamine, välised ja anonüümsed kasutajad Microsoft Teamsi fuajees mööduda, saate seda teha PowerShelli abil. Siin on näide muuta oma organisatsiooni globaalse koosoleku poliitika:

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

See cmdlet-käsk on praegu vaja kasutada Skype Business PowerShelli moodul. Selle cmdlet-käsu kasutamiseks installiprogrammi saamiseks vaadake [haldamine poliitika PowerShelli kaudu](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Saate seadistada uue poliitika, mille peate selle kasutajatele rakendama. Kui muudate Globaalpoliitikat, rakenduvad see automaatselt kasutajatele. Poliitika muutmiseks peate ootama vähemalt 4 tundi ja kuni 24 tundi poliitika jõustumiseks.

Veenduge, et vaadata allpool dokumentatsiooni, enne kui teha need muudatused täpselt aru, mida see võimaldab.

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Fuajeepoliitika juhtelementide koosoleku meeskondade mõistmine

- [Automaatselt tunnistama](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , et inimesed on ühe korraldaja poliitika, mis kontrollib, kas inimesed koosolekuga otse või oodake fuajees, kuni nad on lubatud autenditud kasutaja.

- [Luba anonüümsetel inimestel alustada koosolekut](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) on iga korraldaja poliitika, mis kontrollib, kas anonüümsed inimesed, sealhulgas B2B ja välise kasutajad, saavad liituda kasutaja koosolekuga ilma autenditud kasutaja organisatsioonist osavõtja.

- [Luba dial-in kasutajad mööduda fuajee](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**peatselt**) on ühe korraldaja poliitika, mis kontrollib, kas inimesed, kes dial telefoni liituda otse koosolekule või oodake fuajees, sõltumata **automaatselt tunnistama inimesed** seade.

- [Luba korraldajad alistada fuajeeätted](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **(peatselt**) on ühe korraldaja poliitika, mis kontrollib, kas koosoleku korraldaja saab alistada fuajeesätted, mis admin seatud **automaatselt tunnistama inimesed** ja **lubada dial-in kasutajatel mööduda fuajee** , kui nad ajastada uue koosoleku.

**Märkus:** Lugege [Manage Koosolekupoliitikad meeskonnad](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) täielik ülevaade Microsoft teamsi koosoleku poliitikad.
