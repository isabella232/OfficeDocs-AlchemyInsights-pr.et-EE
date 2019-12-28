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
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889078"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Fuajeeseadete ja meeskondade osalemise taseme kontrollimine

Kui soovite lubada kõigile, sealhulgas dial-in, välised ja anonüümsed kasutajad, et **mööduda fuajee**, kasutada PowerShelli selle ülesande täitmiseks. Siin on näide teie organisatsiooni globaalse koosoleku poliitika muutmise kohta.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

See cmdlet-käsk on praegu vaja kasutada Skype Business PowerShelli moodul. Selle cmdlet-käsu kasutamiseks seadistamiseks vaadake [PowerShelli kaudu haldamine poliitika](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Kui olete poliitika seadistanud, peate selle rakendama kasutajatele; või kui olete muutnud Globaalpoliitikat, rakendatakse seda automaatselt kasutajatele. Mis tahes poliitika muutmiseks peate ootama vähemalt **4 tundi kuni 24 tundi** poliitika jõustumiseks. 

Veenduge, et vaadata allpool dokumentatsiooni, enne kui teha need muudatused täpselt aru, mida see võimaldab.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Fuajeepoliitika juhtelementide koosoleku meeskondade mõistmine

Need sätted kontrollivad, millised osavõtjad ootavad fuajees enne koosoleku lubamist ja koosolekul lubatud osalemise taset. PowerShelli abil saate värskendada koosoleku poliitika sätted, mida pole veel rakendatud (märgistatud "peatselt") meeskonnad halduskeskus. Vaadake allpool näide PowerShelli cmdlet-käsk, mis võimaldab kõigil kasutajatel mööduda fuajee.

- [Automaatselt tunnistama](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , et inimesed on ühe korraldaja poliitika, mis kontrollib, kas inimesed koosolekuga otse või oodake fuajees, kuni nad on lubatud autenditud kasutaja.

- [Luba anonüümsetel inimestel alustada koosolekut](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) on iga korraldaja poliitika, mis kontrollib, kas anonüümsed inimesed, sealhulgas B2B ja välise kasutajad, saavad liituda kasutaja koosolekuga ilma autenditud kasutaja organisatsioonist osavõtja.

- [Luba dial-in kasutajad mööduda fuajee](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**peatselt**) on ühe korraldaja poliitika, mis kontrollib, kas inimesed, kes dial telefoni liituda otse koosolekule või oodake fuajees, sõltumata **automaatselt tunnistama inimesed** seade.

- [Luba korraldajad alistada fuajeeätted](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **(peatselt**) on ühe korraldaja poliitika, mis kontrollib, kas koosoleku korraldaja saab alistada fuajeesätted, mis admin seatud **automaatselt tunnistama inimesed** ja **lubada dial-in kasutajatel mööduda fuajee** , kui nad ajastada uue koosoleku.

**Märkus:** Lugege [Manage Koosolekupoliitikad meeskonnad](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) täielik ülevaade Microsoft teamsi koosoleku poliitikad.
