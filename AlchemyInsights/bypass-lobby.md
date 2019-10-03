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
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="241ed-102">Fuajeeseadete ja osalemise taseme kontrollimine</span><span class="sxs-lookup"><span data-stu-id="241ed-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="241ed-103">Need sätted kontrollivad, millised osavõtjad ootavad fuajees enne koosoleku lubamist ja koosolekul lubatud osalemise taset.</span><span class="sxs-lookup"><span data-stu-id="241ed-103">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="241ed-104">PowerShelli abil saate värskendada koosoleku poliitika sätted, mida pole veel rakendatud (märgistatud "peatselt") meeskonnad halduskeskus.</span><span class="sxs-lookup"><span data-stu-id="241ed-104">You can use Powershell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span>  <span data-ttu-id="241ed-105">Vaadake allpool näide PowerShelli cmdlet-käsk, mis võimaldab kõigil kasutajatel mööduda fuajee.</span><span class="sxs-lookup"><span data-stu-id="241ed-105">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>  

- <span data-ttu-id="241ed-106">[Automaatselt tunnistama](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , et inimesed on ühe korraldaja poliitika, mis kontrollib, kas inimesed koosolekuga otse või oodake fuajees, kuni nad on lubatud autenditud kasutaja.</span><span class="sxs-lookup"><span data-stu-id="241ed-106">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="241ed-107">[Luba anonüümsetel inimestel alustada koosolekut](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) on iga korraldaja poliitika, mis kontrollib, kas anonüümsed inimesed, sealhulgas B2B ja välise kasutajad, saavad liituda kasutaja koosolekuga ilma autenditud kasutaja organisatsioonist osavõtja.</span><span class="sxs-lookup"><span data-stu-id="241ed-107">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="241ed-108">[Luba dial-in kasutajad mööduda fuajee](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**peatselt**) on ühe korraldaja poliitika, mis kontrollib, kas inimesed, kes dial telefoni liituda otse koosolekule või oodake fuajees, sõltumata **automaatselt tunnistama inimesed** seade.</span><span class="sxs-lookup"><span data-stu-id="241ed-108">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="241ed-109">[Luba korraldajad alistada fuajeeätted](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **(peatselt**) on ühe korraldaja poliitika, mis kontrollib, kas koosoleku korraldaja saab alistada fuajeesätted, mis admin seatud **automaatselt tunnistama inimesed** ja **lubada dial-in kasutajatel** uue koosoleku ajastamiseks fuajees mööduda.</span><span class="sxs-lookup"><span data-stu-id="241ed-109">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="241ed-110">**Märkus:** Lugege [Manage Koosolekupoliitikad meeskonnad](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) täielik ülevaade Microsoft teamsi koosoleku poliitikad.</span><span class="sxs-lookup"><span data-stu-id="241ed-110">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span> 


<span data-ttu-id="241ed-111">**PowerShelli näide**</span><span class="sxs-lookup"><span data-stu-id="241ed-111">**PowerShell example**</span></span>

<span data-ttu-id="241ed-112">Kui soovite lubada kõigil, sealhulgas väliste või anonüümsete kasutajate, fuajee mööduda, saate selle ülesande täitmiseks kasutada ka PowerShelli.</span><span class="sxs-lookup"><span data-stu-id="241ed-112">If you'd like to allow everyone, including external or anonymous users, to bypass the lobby, you can also use PowerShell to accomplish this task.</span></span>  <span data-ttu-id="241ed-113">Siin on näide teie organisatsiooni globaalse koosoleku poliitika muutmise kohta.</span><span class="sxs-lookup"><span data-stu-id="241ed-113">Here's an example of modifying the global meeting policy for your organization.</span></span>   

<span data-ttu-id="241ed-114">(Vaadake kindlasti üle ülaltoodud dokumendid enne nende muudatuste tegemist, et mõista täpselt, mida see võimaldab.)</span><span class="sxs-lookup"><span data-stu-id="241ed-114">(Be sure to review the documentation above before making these changes to understand exactly what this allows.)</span></span>

<span data-ttu-id="241ed-115">Set-CsTeamsMeetingPolicy-identiteedi globaalne-AutoAdmittedUsers "kõik"-AllowPSTNUsersToBypassLobby $True</span><span class="sxs-lookup"><span data-stu-id="241ed-115">Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True</span></span>

<span data-ttu-id="241ed-116">Lisateabe saamiseks vaadake [komplekt-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="241ed-116">For more information, see [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span></span>
