---
title: Giphy kasutamine meeskonnatöö vestlustes
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982459"
---
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="86277-102">Giphy kasutamine meeskonnatöö vestlustes</span><span class="sxs-lookup"><span data-stu-id="86277-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="86277-103">Giphy juurdepääs meeskonnatöö vestlusele on vaikimisi lubatud.</span><span class="sxs-lookup"><span data-stu-id="86277-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="86277-104">Administraatorina saate määrata, kas Giphy on kasutajate jaoks saadaval, [häälestades sõnumite saatmise poliitika](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) ning tagades, et **giphy kasutamine vestlustes** on **sisse lülitatud**.</span><span class="sxs-lookup"><span data-stu-id="86277-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="86277-105">Kui gif-töö ei tööta töörühma vestlustes oodatud viisil, siis veenduge, et:</span><span class="sxs-lookup"><span data-stu-id="86277-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="86277-106">[Sõnumite poliitika](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) peab võimaldama giphy.</span><span class="sxs-lookup"><span data-stu-id="86277-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="86277-107">PowerShelli cmdlet-käskude abil kinnitamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="86277-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="86277-108">Veenduge, et saate [hallata PowerShelli abil töörühmi](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="86277-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="86277-109">Käivitage PowerShelli käsk [Get-CsTeamsMessagingPolicy](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) ja veenduge, et **AllowGiphy** oleks seatud väärtusele **True**.</span><span class="sxs-lookup"><span data-stu-id="86277-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="86277-110">Kui **AllowGiphy** väärtuseks on seatud **FALSE** , käivitage järgmine PowerShelli Command [Set-CsTeamsMessagingPolicy-Identity Global-AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="86277-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="86277-111">Giphy URL-ile juurdepääsu lubamiseks peab olema lubatud [Valikuline ühendatud kogemus](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) .</span><span class="sxs-lookup"><span data-stu-id="86277-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="86277-112">Kui teie rentniku jaoks on konfigureeritud mitu töörühma, saate määrata mõjutatud kasutajale määratud poliitika identiteedi, kus on PowerShelli käsk [Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Valige TeamsMessagingPolicy.</span><span class="sxs-lookup"><span data-stu-id="86277-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>
