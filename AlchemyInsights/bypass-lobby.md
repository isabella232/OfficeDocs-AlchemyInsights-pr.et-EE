---
title: Ooteruumist möödumine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820030"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Ooteruumi sätete ja Teamsis osalemise taseme juhtimine

Kui soovite lubada kõigil (sh sissehelistamis-, välis- ja anonüümsetel kasutajatel) ooteruumist mööduda, kasutage selle ülesande täitmiseks PowerShelli. Siin on näide ettevõtte globaalse koosolekupoliitika muutmisest.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

See cmdlet-käsk nõuab praegu Skype'i ärirakenduse PowerShelli mooduli kasutamist. Selle cmdlet-käsu kasutamiseks häälestamiseks vaadake läbi [Poliitikate haldamine PowerShelli kaudu.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)

Kui olete poliitika häälestanud, peate selle kasutajatele rakendama; või kui olete muutnud globaalset poliitikat, rakendub see kasutajatele automaatselt. Poliitika muutmiseks peate poliitikate jõustumist ootama vähemalt 4 tundi kuni **24** tundi. 

Enne muudatuste tegemist vaadake kindlasti läbi allolevad dokumendid, et mõista täpselt, mida see võimaldab.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Teamsi koosoleku ooteruumipoliitika juhtelementide mõistmine

Nende sätete abil saate kontrollida, millised koosolekul osalejad ooteruumis ootavad, enne kui nad koosolekule lubatakse, ja koosolekul osalemise taset. PowerShelli abil saate värskendada Teamsi halduskeskuses veel rakendamata koosolekupoliitika sätteid (sildiga "peagi tulekul"). Vaadake allpool powerShelli cmdlet-käsku, mis võimaldab kõigil kasutajatel ooteruumist mööda minna.

- [Inimeste automaatne vastuvõtt](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) on korraldaja poliitika, mis määrab, kas inimesed liituvad koosolekuga otse või ootavad ooteruumis, kuni autenditud kasutaja on nad vastu võtmas.

- [Anonüümsete inimeste](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) koosoleku alustamiseks on korraldaja poliitika, mis määrab, kas anonüümsed inimesed (sh B2B ja liitkasutajad) saavad liituda kasutaja koosolekuga ilma ettevõtte autenditud kasutajata.

- [Luba sissehelistamiskasutajatel](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) ooteruumist **mööduda**(peagi tulekul) on korraldaja poliitika, mis määrab, kas telefoni teel sissehelistavad inimesed liituvad koosolekuga otse või ootavad ooteruumis, sõltumata sättest **"Luba automaatselt inimesi".**

- [Korraldajatel](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) ooteruumisätete **(peagi** tulekul) alistamine on korraldaja poliitika, mis määrab, kas koosoleku korraldaja saab  alistada ooteruumisätted, mille administraator on määranud jaotises Inimeste automaatne vastuvõtt ja Luba sissehelistamiskasutajatel uue koosoleku plaanimisel ooteruumist mööduda. 

**Märkus.** Lisateavet [Microsoft Teamsi koosolekupoliitikate](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) täieliku ülevaate kohta lugege artiklist Koosolekute poliitikate haldamine Teamsis.
