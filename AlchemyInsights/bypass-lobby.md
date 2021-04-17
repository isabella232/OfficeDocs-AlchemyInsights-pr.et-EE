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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="ea850-102">Ooteruumi sätete ja Teamsis osalemise taseme juhtimine</span><span class="sxs-lookup"><span data-stu-id="ea850-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="ea850-103">Kui soovite lubada kõigil (sh sissehelistamis-, välis- ja anonüümsetel kasutajatel) ooteruumist mööduda, kasutage selle ülesande täitmiseks PowerShelli.</span><span class="sxs-lookup"><span data-stu-id="ea850-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="ea850-104">Siin on näide ettevõtte globaalse koosolekupoliitika muutmisest.</span><span class="sxs-lookup"><span data-stu-id="ea850-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="ea850-105">See cmdlet-käsk nõuab praegu Skype'i ärirakenduse PowerShelli mooduli kasutamist.</span><span class="sxs-lookup"><span data-stu-id="ea850-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="ea850-106">Selle cmdlet-käsu kasutamiseks häälestamiseks vaadake läbi [Poliitikate haldamine PowerShelli kaudu.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)</span><span class="sxs-lookup"><span data-stu-id="ea850-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="ea850-107">Kui olete poliitika häälestanud, peate selle kasutajatele rakendama; või kui olete muutnud globaalset poliitikat, rakendub see kasutajatele automaatselt.</span><span class="sxs-lookup"><span data-stu-id="ea850-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="ea850-108">Poliitika muutmiseks peate poliitikate jõustumist ootama vähemalt 4 tundi kuni **24** tundi.</span><span class="sxs-lookup"><span data-stu-id="ea850-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="ea850-109">Enne muudatuste tegemist vaadake kindlasti läbi allolevad dokumendid, et mõista täpselt, mida see võimaldab.</span><span class="sxs-lookup"><span data-stu-id="ea850-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="ea850-110">Teamsi koosoleku ooteruumipoliitika juhtelementide mõistmine</span><span class="sxs-lookup"><span data-stu-id="ea850-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="ea850-111">Nende sätete abil saate kontrollida, millised koosolekul osalejad ooteruumis ootavad, enne kui nad koosolekule lubatakse, ja koosolekul osalemise taset.</span><span class="sxs-lookup"><span data-stu-id="ea850-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="ea850-112">PowerShelli abil saate värskendada Teamsi halduskeskuses veel rakendamata koosolekupoliitika sätteid (sildiga "peagi tulekul").</span><span class="sxs-lookup"><span data-stu-id="ea850-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="ea850-113">Vaadake allpool powerShelli cmdlet-käsku, mis võimaldab kõigil kasutajatel ooteruumist mööda minna.</span><span class="sxs-lookup"><span data-stu-id="ea850-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="ea850-114">[Inimeste automaatne vastuvõtt](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) on korraldaja poliitika, mis määrab, kas inimesed liituvad koosolekuga otse või ootavad ooteruumis, kuni autenditud kasutaja on nad vastu võtmas.</span><span class="sxs-lookup"><span data-stu-id="ea850-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="ea850-115">[Anonüümsete inimeste](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) koosoleku alustamiseks on korraldaja poliitika, mis määrab, kas anonüümsed inimesed (sh B2B ja liitkasutajad) saavad liituda kasutaja koosolekuga ilma ettevõtte autenditud kasutajata.</span><span class="sxs-lookup"><span data-stu-id="ea850-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="ea850-116">[Luba sissehelistamiskasutajatel](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) ooteruumist **mööduda**(peagi tulekul) on korraldaja poliitika, mis määrab, kas telefoni teel sissehelistavad inimesed liituvad koosolekuga otse või ootavad ooteruumis, sõltumata sättest **"Luba automaatselt inimesi".**</span><span class="sxs-lookup"><span data-stu-id="ea850-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="ea850-117">[Korraldajatel](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) ooteruumisätete **(peagi** tulekul) alistamine on korraldaja poliitika, mis määrab, kas koosoleku korraldaja saab  alistada ooteruumisätted, mille administraator on määranud jaotises Inimeste automaatne vastuvõtt ja Luba sissehelistamiskasutajatel uue koosoleku plaanimisel ooteruumist mööduda. </span><span class="sxs-lookup"><span data-stu-id="ea850-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="ea850-118">**Märkus.** Lisateavet [Microsoft Teamsi koosolekupoliitikate](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) täieliku ülevaate kohta lugege artiklist Koosolekute poliitikate haldamine Teamsis.</span><span class="sxs-lookup"><span data-stu-id="ea850-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
