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
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="83a72-102">Fuajeeseadete ja osalemise taseme kontrollimine</span><span class="sxs-lookup"><span data-stu-id="83a72-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="83a72-103">Kui soovite lubada kõigil, sealhulgas dial-in, välised ja anonüümsed kasutajad mööduda fuajee, saate seda teha PowerShelli abil.</span><span class="sxs-lookup"><span data-stu-id="83a72-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby, you can use PowerShell to do it.</span></span> <span data-ttu-id="83a72-104">Siin on näide muuta oma organisatsiooni globaalse koosoleku poliitika:</span><span class="sxs-lookup"><span data-stu-id="83a72-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="83a72-105">See cmdlet-käsk on praegu vaja kasutada Skype Business PowerShelli moodul.</span><span class="sxs-lookup"><span data-stu-id="83a72-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="83a72-106">Selle cmdlet-käsu kasutamiseks installiprogrammi saamiseks vaadake [haldamine poliitika PowerShelli kaudu](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="83a72-106">To get setup to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="83a72-107">Saate seadistada uue poliitika, mille peate selle kasutajatele rakendama.</span><span class="sxs-lookup"><span data-stu-id="83a72-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="83a72-108">Kui muudate Globaalpoliitikat, rakenduvad see automaatselt kasutajatele.</span><span class="sxs-lookup"><span data-stu-id="83a72-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="83a72-109">Poliitika muutmiseks peate ootama vähemalt 4 tundi ja kuni 24 tundi poliitika jõustumiseks.</span><span class="sxs-lookup"><span data-stu-id="83a72-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="83a72-110">Veenduge, et vaadata allpool dokumentatsiooni, enne kui teha need muudatused täpselt aru, mida see võimaldab.</span><span class="sxs-lookup"><span data-stu-id="83a72-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="83a72-111">Fuajeepoliitika juhtelementide koosoleku meeskondade mõistmine</span><span class="sxs-lookup"><span data-stu-id="83a72-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="83a72-112">[Automaatselt tunnistama](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , et inimesed on ühe korraldaja poliitika, mis kontrollib, kas inimesed koosolekuga otse või oodake fuajees, kuni nad on lubatud autenditud kasutaja.</span><span class="sxs-lookup"><span data-stu-id="83a72-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="83a72-113">[Luba anonüümsetel inimestel alustada koosolekut](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) on iga korraldaja poliitika, mis kontrollib, kas anonüümsed inimesed, sealhulgas B2B ja välise kasutajad, saavad liituda kasutaja koosolekuga ilma autenditud kasutaja organisatsioonist osavõtja.</span><span class="sxs-lookup"><span data-stu-id="83a72-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="83a72-114">[Luba dial-in kasutajad mööduda fuajee](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**peatselt**) on ühe korraldaja poliitika, mis kontrollib, kas inimesed, kes dial telefoni liituda otse koosolekule või oodake fuajees, sõltumata **automaatselt tunnistama inimesed** seade.</span><span class="sxs-lookup"><span data-stu-id="83a72-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="83a72-115">[Luba korraldajad alistada fuajeeätted](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **(peatselt**) on ühe korraldaja poliitika, mis kontrollib, kas koosoleku korraldaja saab alistada fuajeesätted, mis admin seatud **automaatselt tunnistama inimesed** ja **lubada dial-in kasutajatel** uue koosoleku ajastamiseks fuajees mööduda.</span><span class="sxs-lookup"><span data-stu-id="83a72-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="83a72-116">**Märkus:** Lugege [Manage Koosolekupoliitikad meeskonnad](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) täielik ülevaade Microsoft teamsi koosoleku poliitikad.</span><span class="sxs-lookup"><span data-stu-id="83a72-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
