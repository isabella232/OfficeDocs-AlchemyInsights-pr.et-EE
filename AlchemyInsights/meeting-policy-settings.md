---
title: Poliitikasätete koosolek
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: b5599c9974eb1c112835a9f42e4ebdc926071ea2
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627570"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="9358b-102">Microsoft Teamsi koosolekupoliitikate haldamine</span><span class="sxs-lookup"><span data-stu-id="9358b-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="9358b-103">Koosolekupoliitikaid kasutatakse nende funktsioonide juhtimiseks, mis on saadaval osavõtjatele koosolekuteks, mis on planeeritud teie organisatsiooni kasutajate poolt.</span><span class="sxs-lookup"><span data-stu-id="9358b-103">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="9358b-104">Mõned koosolekupoliitikate funktsioonid ei pruugi veel meeskondi administreerimiskeskuses rakendada (need on dokumentatsioonis märgistatud "peatselt").</span><span class="sxs-lookup"><span data-stu-id="9358b-104">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="9358b-105">Sel juhul või kui saate tõrketeate, nagu "me ei saa värskendada poliitika kohe, kuid proovige seda hiljem uuesti" Microsoft Teams halduskeskus, soovitame kasutada PowerShelli luua või muuta meeskondade koosolekute poliitikad.</span><span class="sxs-lookup"><span data-stu-id="9358b-105">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="9358b-106">Koosolekupoliitikate kohta lisateabe saamiseks vaadake järgmisi ressursse:</span><span class="sxs-lookup"><span data-stu-id="9358b-106">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="9358b-107">Poliitikate loomise, muutuste tegemise ja poliitika kasutajate määramise kohta leiate teavet teemast [teamsi koosolekute poliitikate haldamine](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="9358b-107">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="9358b-108">Poliitika muudatuste tegemiseks PowerShelli cmdlet-käskude abil vaadake teemat [Teamsi PowerShelli ülevaade](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="9358b-108">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="9358b-109">Peate kasutama [Skype Business PowerShelli moodul](https://www.microsoft.com/download/details.aspx?id=39366) meeskonnad koosoleku poliitika.</span><span class="sxs-lookup"><span data-stu-id="9358b-109">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="9358b-110">Vaadake üle [\*-csteamsmeetingpolicy cmdlet-käskude dokumentatsiooni](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) lisateabe saamiseks.</span><span class="sxs-lookup"><span data-stu-id="9358b-110">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

<span data-ttu-id="9358b-111">**Märkus:** Poliitika muudatuste jõustumiseks kasutajatele võib kuluda kuni 24 tundi.</span><span class="sxs-lookup"><span data-stu-id="9358b-111">**Note:** It can take up to 24 hours for policy changes to take effect for users.</span></span> <span data-ttu-id="9358b-112">Võimalik, et te ei saa äsja loodud poliitikaid kohe muuta; Oodake 4 tundi ja proovige äsja loodud poliitikat uuesti muuta.</span><span class="sxs-lookup"><span data-stu-id="9358b-112">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span> <span data-ttu-id="9358b-113">Kui teil on endiselt probleeme, proovige PowerShelli.</span><span class="sxs-lookup"><span data-stu-id="9358b-113">If you're still having problems, try PowerShell.</span></span>  