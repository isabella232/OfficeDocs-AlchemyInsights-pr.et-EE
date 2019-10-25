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
ms.openlocfilehash: 6632bb0c09c7ce99f14cd55582025b37a846369d
ms.sourcegitcommit: ee719f011f766fc20d23e935e98d7e33c326183b
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/24/2019
ms.locfileid: "37654252"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Fuajeeseadete ja osalemise taseme kontrollimine

Kui soovite lubada kõigil, sealhulgas dial-in, välised ja anonüümsed kasutajad mööduda fuajee, saate seda teha PowerShelli abil. Siin on näide muuta oma organisatsiooni globaalse koosoleku poliitika:

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

See cmdlet-käsk on praegu vaja kasutada Skype Business PowerShelli moodul. Selle cmdlet-käsu kasutamiseks installiprogrammi saamiseks vaadake [haldamine poliitika PowerShelli kaudu](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Saate seadistada uue poliitika, mille peate selle kasutajatele rakendama. Kui muudate Globaalpoliitikat, rakenduvad see automaatselt kasutajatele. Poliitika muutmiseks peate ootama vähemalt 4 tundi ja kuni 24 tundi poliitika jõustumiseks.

Veenduge, et vaadata allpool dokumentatsiooni, enne kui teha need muudatused täpselt aru, mida see võimaldab.

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Fuajeepoliitika juhtelementide koosoleku meeskondade mõistmine

- [Automaatselt tunnistama](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , et inimesed on ühe korraldaja poliitika, mis kontrollib, kas inimesed koosolekuga otse või oodake fuajees, kuni nad on lubatud autenditud kasutaja.

- [Luba anonüümsetel inimestel alustada koosolekut](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) on iga korraldaja poliitika, mis kontrollib, kas anonüümsed inimesed, sealhulgas B2B ja välise kasutajad, saavad liituda kasutaja koosolekuga ilma autenditud kasutaja organisatsioonist osavõtja.

- [Luba dial-in kasutajad mööduda fuajee](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**peatselt**) on ühe korraldaja poliitika, mis kontrollib, kas inimesed, kes dial telefoni liituda otse koosolekule või oodake fuajees, sõltumata **automaatselt tunnistama inimesed** seade.

- [Luba korraldajad alistada fuajeeätted](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **(peatselt**) on ühe korraldaja poliitika, mis kontrollib, kas koosoleku korraldaja saab alistada fuajeesätted, mis admin seatud **automaatselt tunnistama inimesed** ja **lubada dial-in kasutajatel** uue koosoleku ajastamiseks fuajees mööduda.

**Märkus:** Lugege [Manage Koosolekupoliitikad meeskonnad](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) täielik ülevaade Microsoft teamsi koosoleku poliitikad.
