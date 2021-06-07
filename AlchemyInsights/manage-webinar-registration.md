---
title: Veebisenaride registreerimise haldamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793709"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="2cb2b-102">Veebisenaride registreerimise haldamine</span><span class="sxs-lookup"><span data-stu-id="2cb2b-102">Manage webinar registration</span></span>

<span data-ttu-id="2cb2b-103">PowerShelli käskude abil saate Teams veebiportaalide Teams kasutajaks registreeruda.</span><span class="sxs-lookup"><span data-stu-id="2cb2b-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="2cb2b-104">PowerShelli Teams leiate teemast [Teams PowerShell](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="2cb2b-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="2cb2b-105">Vaikimisi on *WhoCanRegister* lubatud ja selle väärtuseks on seatud **EveryoneInCompany**.</span><span class="sxs-lookup"><span data-stu-id="2cb2b-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="2cb2b-106">Selleks et lubada kõigil (sh anonüümsetel kasutajatel) registreeruda, peate powershelli käsu abil määrama koosolekupoliitika väärtuseks Kõik. </span><span class="sxs-lookup"><span data-stu-id="2cb2b-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="2cb2b-107">**Märkus.** Kui anonüümne liitumine on koosolekusätetes välja lülitatud, ei saa anonüümsed kasutajad veebiseinaritega liituda.</span><span class="sxs-lookup"><span data-stu-id="2cb2b-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="2cb2b-108">Lisateavet ja selle sätte lubamise kohta leiate teemast [Koosolekusätete haldamine Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span><span class="sxs-lookup"><span data-stu-id="2cb2b-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="2cb2b-109">Kui soovite koosoleku registreerimise välja lülitada, määrake *allowMeetingRegistration väärtuseks* **False (Väär).**</span><span class="sxs-lookup"><span data-stu-id="2cb2b-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="2cb2b-110">Lisateavet selle kohta, kes saab veebiseinarite jaoks registreeruda, leiate teemast [Webinarsi kasutajaks registreerujate konfigureerimine.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)</span><span class="sxs-lookup"><span data-stu-id="2cb2b-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="2cb2b-111">Lisateavet Microsofti loendite sätete kohta leiate teemast [Microsofti loendite sätete juhtimine.](/sharepoint/control-lists)</span><span class="sxs-lookup"><span data-stu-id="2cb2b-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
