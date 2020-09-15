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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="1621b-102">Fuajee seadete reguleerimine ja meeskonnas osalemise tase</span><span class="sxs-lookup"><span data-stu-id="1621b-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="1621b-103">Kui soovite lubada kõigil (sh sissehelistamine, välised ja anonüümsed kasutajad **) fuajeest**loobuda, kasutage selle ülesande saavutamiseks PowerShelli.</span><span class="sxs-lookup"><span data-stu-id="1621b-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="1621b-104">Siin on näide organisatsiooni globaalse koosoleku poliitika muutmisest.</span><span class="sxs-lookup"><span data-stu-id="1621b-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="1621b-105">See cmdlet-käsk nõuab praegu Skype ' i ärirakenduse PowerShelli mooduli kasutamist.</span><span class="sxs-lookup"><span data-stu-id="1621b-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="1621b-106">Selle cmdlet-käsu kasutamiseks häälestamiseks uurige [PowerShelli kaudu halduse poliitikaid](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="1621b-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="1621b-107">Kui olete poliitika häälestanud, peate selle rakendama kasutajatele; Kui olete muutnud globaalset poliitikat, rakendub see automaatselt kasutajatele.</span><span class="sxs-lookup"><span data-stu-id="1621b-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="1621b-108">Poliitikate muutmise korral peate poliitika jõustumiseks ootama vähemalt **4 tundi kuni 24 tundi** .</span><span class="sxs-lookup"><span data-stu-id="1621b-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="1621b-109">Enne nende muudatuste tegemist lugege kindlasti allpool olevad dokumendid üle, et mõista täpselt, mida see võimaldab.</span><span class="sxs-lookup"><span data-stu-id="1621b-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="1621b-110">Töörühmade koosolekul olevate lobby poliitika juhtelementide mõistmine</span><span class="sxs-lookup"><span data-stu-id="1621b-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="1621b-111">Need sätted, mida koosolekul osalejad ootavad fuajees enne, kui nad on koosolekule sisse lubatud ja koosolekul lubatud osalemise tase.</span><span class="sxs-lookup"><span data-stu-id="1621b-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="1621b-112">PowerShelli abil saate värskendada koosolekute poliitika sätteid, mida pole veel rakendatud (sildistatud "peagi") meeskonnatöö administreerimiskeskuses.</span><span class="sxs-lookup"><span data-stu-id="1621b-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="1621b-113">Siit leiate teavet PowerShelli cmdlet-käsu kohta, mis võimaldab kõigil kasutajatel fuajeest mööduda.</span><span class="sxs-lookup"><span data-stu-id="1621b-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="1621b-114">Saate [automaatselt tunnistada](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , et inimesed on korraldaja poliitika, mis määrab, kas inimesed liituvad koosolekuga otse või ootavad fuajees, kuni need on autenditud kasutaja poolt vastu võetud.</span><span class="sxs-lookup"><span data-stu-id="1621b-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="1621b-115">[Luba anonüümsetel inimestel koosolekut alustada](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) on korraldaja poliitika, mis määrab, kas anonüümsed inimesed (sh B2B ja väliskasutajad) saavad liituda kasutaja koosolekuga, kasutaja koosolekul ei ole autentimata kasutajat.</span><span class="sxs-lookup"><span data-stu-id="1621b-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="1621b-116">[Luba sissehelistamise kasutajatel fuajeest mööda hiilida](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**tulekul**) on ühe korraldaja poliitika, mis määrab, kas telefoni teel sissehelistavad inimesed liituvad koosolekuga otse või ootavad fuajees, sõltumata sellest, kas see säte on **automaatselt** keelatud.</span><span class="sxs-lookup"><span data-stu-id="1621b-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="1621b-117">[Luba korraldajatel lobby sätteid alistada](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**tulekul**) on korraldaja poliitika, mis määrab, kas koosoleku korraldaja saab alistada nende lobby-sätted, mille administraator on määranud **automaatselt tunnistama** , ja **lubada sissehelistamise kasutajatel minna fuajeest mööda,** kui nad plaanivad uut koosolekut.</span><span class="sxs-lookup"><span data-stu-id="1621b-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="1621b-118">**Märkus:** Lugege jaotist [koosolekute poliitikate haldamine töörühmades](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) Microsoft teamsi koosolekute poliitikate tervikliku ülevaate saamiseks.</span><span class="sxs-lookup"><span data-stu-id="1621b-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
