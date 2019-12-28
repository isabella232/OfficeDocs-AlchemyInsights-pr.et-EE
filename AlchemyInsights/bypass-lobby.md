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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="3dbdc-102">Fuajeeseadete ja meeskondade osalemise taseme kontrollimine</span><span class="sxs-lookup"><span data-stu-id="3dbdc-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="3dbdc-103">Kui soovite lubada kõigile, sealhulgas dial-in, välised ja anonüümsed kasutajad, et **mööduda fuajee**, kasutada PowerShelli selle ülesande täitmiseks.</span><span class="sxs-lookup"><span data-stu-id="3dbdc-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="3dbdc-104">Siin on näide teie organisatsiooni globaalse koosoleku poliitika muutmise kohta.</span><span class="sxs-lookup"><span data-stu-id="3dbdc-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="3dbdc-105">See cmdlet-käsk on praegu vaja kasutada Skype Business PowerShelli moodul.</span><span class="sxs-lookup"><span data-stu-id="3dbdc-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="3dbdc-106">Selle cmdlet-käsu kasutamiseks seadistamiseks vaadake [PowerShelli kaudu haldamine poliitika](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="3dbdc-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="3dbdc-107">Kui olete poliitika seadistanud, peate selle rakendama kasutajatele; või kui olete muutnud Globaalpoliitikat, rakendatakse seda automaatselt kasutajatele.</span><span class="sxs-lookup"><span data-stu-id="3dbdc-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="3dbdc-108">Mis tahes poliitika muutmiseks peate ootama vähemalt **4 tundi kuni 24 tundi** poliitika jõustumiseks.</span><span class="sxs-lookup"><span data-stu-id="3dbdc-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="3dbdc-109">Veenduge, et vaadata allpool dokumentatsiooni, enne kui teha need muudatused täpselt aru, mida see võimaldab.</span><span class="sxs-lookup"><span data-stu-id="3dbdc-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="3dbdc-110">Fuajeepoliitika juhtelementide koosoleku meeskondade mõistmine</span><span class="sxs-lookup"><span data-stu-id="3dbdc-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="3dbdc-111">Need sätted kontrollivad, millised osavõtjad ootavad fuajees enne koosoleku lubamist ja koosolekul lubatud osalemise taset.</span><span class="sxs-lookup"><span data-stu-id="3dbdc-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="3dbdc-112">PowerShelli abil saate värskendada koosoleku poliitika sätted, mida pole veel rakendatud (märgistatud "peatselt") meeskonnad halduskeskus.</span><span class="sxs-lookup"><span data-stu-id="3dbdc-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="3dbdc-113">Vaadake allpool näide PowerShelli cmdlet-käsk, mis võimaldab kõigil kasutajatel mööduda fuajee.</span><span class="sxs-lookup"><span data-stu-id="3dbdc-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="3dbdc-114">[Automaatselt tunnistama](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , et inimesed on ühe korraldaja poliitika, mis kontrollib, kas inimesed koosolekuga otse või oodake fuajees, kuni nad on lubatud autenditud kasutaja.</span><span class="sxs-lookup"><span data-stu-id="3dbdc-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="3dbdc-115">[Luba anonüümsetel inimestel alustada koosolekut](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) on iga korraldaja poliitika, mis kontrollib, kas anonüümsed inimesed, sealhulgas B2B ja välise kasutajad, saavad liituda kasutaja koosolekuga ilma autenditud kasutaja organisatsioonist osavõtja.</span><span class="sxs-lookup"><span data-stu-id="3dbdc-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="3dbdc-116">[Luba dial-in kasutajad mööduda fuajee](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**peatselt**) on ühe korraldaja poliitika, mis kontrollib, kas inimesed, kes dial telefoni liituda otse koosolekule või oodake fuajees, sõltumata **automaatselt tunnistama inimesed** seade.</span><span class="sxs-lookup"><span data-stu-id="3dbdc-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="3dbdc-117">[Luba korraldajad alistada fuajeeätted](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **(peatselt**) on ühe korraldaja poliitika, mis kontrollib, kas koosoleku korraldaja saab alistada fuajeesätted, mis admin seatud **automaatselt tunnistama inimesed** ja **lubada dial-in kasutajatel mööduda fuajee** , kui nad ajastada uue koosoleku.</span><span class="sxs-lookup"><span data-stu-id="3dbdc-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="3dbdc-118">**Märkus:** Lugege [Manage Koosolekupoliitikad meeskonnad](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) täielik ülevaade Microsoft teamsi koosoleku poliitikad.</span><span class="sxs-lookup"><span data-stu-id="3dbdc-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
