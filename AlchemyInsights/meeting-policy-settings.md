---
title: Koosolekute poliitika sätted
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
- "9000734"
- "2657"
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794330"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="19908-102">Microsoft Teamsi koosolekute poliitikate haldamine</span><span class="sxs-lookup"><span data-stu-id="19908-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="19908-103">**Märkus: poliitika muudatuste jõustamiseks kasutajate jaoks võib kuluda kuni 24 tundi.**</span><span class="sxs-lookup"><span data-stu-id="19908-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="19908-104">Võimalik, et te ei saa kohe vastloodud poliitikaid muuta; Oodake 4 tundi ja proovige uuesti uuesti loodud poliitikat muuta.</span><span class="sxs-lookup"><span data-stu-id="19908-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="19908-105">Koosoleku põhimõtteid kasutatakse selliste funktsioonide juhtimiseks, mis on saadaval koosolekul osalejatele koosolekul, mis on planeeritud teie asutuse kasutajate jaoks.</span><span class="sxs-lookup"><span data-stu-id="19908-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="19908-106">Mõned koosolekute poliitikate funktsioonid ei pruugi olla meeskonnatöö administreerimiskeskuses veel saadaval (need on dokumentides "Varsti tulekul").</span><span class="sxs-lookup"><span data-stu-id="19908-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="19908-107">Sellisel juhul või kui teile kuvatakse tõrketeade "me ei saa praegu poliitikat värskendada, kuid proovige seda hiljem uuesti" Microsoft Teamsi administreerimiskeskuses, soovitame kasutada PowerShelli, et luua või muuta meeskonnatöö koosoleku poliitikaid.</span><span class="sxs-lookup"><span data-stu-id="19908-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="19908-108">Lisateavet koosolekute poliitikate kohta leiate järgmistest allikatest.</span><span class="sxs-lookup"><span data-stu-id="19908-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="19908-109">Lisateavet poliitikate loomise, muudatuste tegemise ja kasutajate poliitikale määramise kohta leiate teemast [koosolekute poliitikate haldamine töörühmades](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="19908-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="19908-110">PowerShelli cmdlet-käskude abil poliitika muudatuste tegemiseks lugege teemat [teamsi PowerShelli ülevaade](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="19908-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="19908-111">Meeskonnatöö koosoleku poliitikate jaoks peate kasutama [Skype ' i ärirakenduse PowerShelli moodulit](https://www.microsoft.com/download/details.aspx?id=39366) .</span><span class="sxs-lookup"><span data-stu-id="19908-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="19908-112">Lisateavet leiate [\*-CsTeamsMeetingPolicy cmdlet-käskude dokumentatsioonist](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) .</span><span class="sxs-lookup"><span data-stu-id="19908-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

