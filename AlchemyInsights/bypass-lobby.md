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
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376609"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Fuajeeseadete ja osalemise taseme kontrollimine

Need sätted kontrollivad, millised osavõtjad ootavad fuajees enne koosoleku lubamist ja koosolekul lubatud osalemise taset. PowerShelli abil saate värskendada koosoleku poliitika sätted, mida pole veel rakendatud (märgistatud "peatselt") meeskonnad halduskeskus.  Vaadake allpool näide PowerShelli cmdlet-käsk, mis võimaldab kõigil kasutajatel mööduda fuajee.  

- [Automaatselt tunnistama](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , et inimesed on ühe korraldaja poliitika, mis kontrollib, kas inimesed koosolekuga otse või oodake fuajees, kuni nad on lubatud autenditud kasutaja.

- [Luba anonüümsetel inimestel alustada koosolekut](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) on iga korraldaja poliitika, mis kontrollib, kas anonüümsed inimesed, sealhulgas B2B ja välise kasutajad, saavad liituda kasutaja koosolekuga ilma autenditud kasutaja organisatsioonist osavõtja.

- [Luba dial-in kasutajad mööduda fuajee](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**peatselt**) on ühe korraldaja poliitika, mis kontrollib, kas inimesed, kes dial telefoni liituda otse koosolekule või oodake fuajees, sõltumata **automaatselt tunnistama inimesed** seade.

- [Luba korraldajad alistada fuajeeätted](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **(peatselt**) on ühe korraldaja poliitika, mis kontrollib, kas koosoleku korraldaja saab alistada fuajeesätted, mis admin seatud **automaatselt tunnistama inimesed** ja **lubada dial-in kasutajatel** uue koosoleku ajastamiseks fuajees mööduda.

**Märkus:** Lugege [Manage Koosolekupoliitikad meeskonnad](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) täielik ülevaade Microsoft teamsi koosoleku poliitikad. 


**PowerShelli näide**

Kui soovite lubada kõigil, sealhulgas väliste või anonüümsete kasutajate, fuajee mööduda, saate selle ülesande täitmiseks kasutada ka PowerShelli.  Siin on näide teie organisatsiooni globaalse koosoleku poliitika muutmise kohta.   

(Vaadake kindlasti üle ülaltoodud dokumendid enne nende muudatuste tegemist, et mõista täpselt, mida see võimaldab.)

Set-CsTeamsMeetingPolicy-identiteedi globaalne-AutoAdmittedUsers "kõik"-AllowPSTNUsersToBypassLobby $True

Lisateabe saamiseks vaadake [komplekt-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).
