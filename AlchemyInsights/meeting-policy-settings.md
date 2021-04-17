---
title: Koosolekupoliitika sätted
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
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825439"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="65a21-102">Microsoft Teamsi koosolekukutsete haldamine</span><span class="sxs-lookup"><span data-stu-id="65a21-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="65a21-103">**Märkus. Poliitikamuudatuste kasutajate jaoks jõustumist võib võtta kuni 24 tundi.**</span><span class="sxs-lookup"><span data-stu-id="65a21-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="65a21-104">Võimalik, et te ei saa vastloodud poliitikaid kohe muuta; oodake 4 tundi ja proovige uuesti loodud poliitikat muuta.</span><span class="sxs-lookup"><span data-stu-id="65a21-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="65a21-105">Koosolekupoliitikaid kasutatakse nende funktsioonide tõrjeks, mis on koosolekul osalejatele saadaval teie asutuse kasutajate ajastatud koosolekute jaoks.</span><span class="sxs-lookup"><span data-stu-id="65a21-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="65a21-106">Mõnda koosolekupoliitika funktsioone ei pruugita Teamsi halduskeskuses veel rakendada (need on dokumentatsioonis sildiga "peagi tulekul").</span><span class="sxs-lookup"><span data-stu-id="65a21-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="65a21-107">Sel juhul või kui teile kuvatakse Microsoft Teamsi halduskeskuses tõrketeade "Me ei saa poliitikat praegu värskendada, kuid proovige seda hiljem uuesti", soovitame kasutada PowerShelli Teamsi koosolekupoliitikate loomiseks või muutmiseks.</span><span class="sxs-lookup"><span data-stu-id="65a21-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="65a21-108">Lisateavet koosolekupoliitikate kohta leiate järgmistest ressurssidest.</span><span class="sxs-lookup"><span data-stu-id="65a21-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="65a21-109">Lisateavet poliitikate loomise, muudatuste tegemise ja poliitikale kasutajate määramise kohta leiate teemast [Teamsi koosolekupoliitikate haldamine.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="65a21-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="65a21-110">PowerShelli cmdlet-käskude abil poliitika muutmiseks lugege teemat [Teamsi PowerShelli ülevaade](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="65a21-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="65a21-111">Teamsi koosolekupoliitikate [jaoks peate kasutama Skype'i ärirakenduse PowerShelli](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) moodulit.</span><span class="sxs-lookup"><span data-stu-id="65a21-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="65a21-112">Vaadake [lisateavet cmdlet-käskude \*-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) dokumentatsioonist.</span><span class="sxs-lookup"><span data-stu-id="65a21-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

