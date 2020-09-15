---
title: Bypass lobby
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684946"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Fuajee seadete reguleerimine ja meeskonnas osalemise tase

Kui soovite lubada kõigil (sh sissehelistamine, välised ja anonüümsed kasutajad **) fuajeest**loobuda, kasutage selle ülesande saavutamiseks PowerShelli. Siin on näide organisatsiooni globaalse koosoleku poliitika muutmisest.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

See cmdlet-käsk nõuab praegu Skype ' i ärirakenduse PowerShelli mooduli kasutamist. Selle cmdlet-käsu kasutamiseks häälestamiseks uurige [PowerShelli kaudu halduse poliitikaid](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Kui olete poliitika häälestanud, peate selle rakendama kasutajatele; Kui olete muutnud globaalset poliitikat, rakendub see automaatselt kasutajatele. Poliitikate muutmise korral peate poliitika jõustumiseks ootama vähemalt **4 tundi kuni 24 tundi** . 

Enne nende muudatuste tegemist lugege kindlasti allpool olevad dokumendid üle, et mõista täpselt, mida see võimaldab.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Töörühmade koosolekul olevate lobby poliitika juhtelementide mõistmine

Need sätted, mida koosolekul osalejad ootavad fuajees enne, kui nad on koosolekule sisse lubatud ja koosolekul lubatud osalemise tase. PowerShelli abil saate värskendada koosolekute poliitika sätteid, mida pole veel rakendatud (sildistatud "peagi") meeskonnatöö administreerimiskeskuses. Siit leiate teavet PowerShelli cmdlet-käsu kohta, mis võimaldab kõigil kasutajatel fuajeest mööduda.

- Saate [automaatselt tunnistada](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , et inimesed on korraldaja poliitika, mis määrab, kas inimesed liituvad koosolekuga otse või ootavad fuajees, kuni need on autenditud kasutaja poolt vastu võetud.

- [Luba anonüümsetel inimestel koosolekut alustada](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) on korraldaja poliitika, mis määrab, kas anonüümsed inimesed (sh B2B ja väliskasutajad) saavad liituda kasutaja koosolekuga, kasutaja koosolekul ei ole autentimata kasutajat.

- [Luba sissehelistamise kasutajatel fuajeest mööda hiilida](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**tulekul**) on ühe korraldaja poliitika, mis määrab, kas telefoni teel sissehelistavad inimesed liituvad koosolekuga otse või ootavad fuajees, sõltumata sellest, kas see säte on **automaatselt** keelatud.

- [Luba korraldajatel lobby sätteid alistada](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**tulekul**) on korraldaja poliitika, mis määrab, kas koosoleku korraldaja saab alistada nende lobby-sätted, mille administraator on määranud **automaatselt tunnistama** , ja **lubada sissehelistamise kasutajatel minna fuajeest mööda,** kui nad plaanivad uut koosolekut.

**Märkus:** Lugege jaotist [koosolekute poliitikate haldamine töörühmades](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) Microsoft teamsi koosolekute poliitikate tervikliku ülevaate saamiseks.
