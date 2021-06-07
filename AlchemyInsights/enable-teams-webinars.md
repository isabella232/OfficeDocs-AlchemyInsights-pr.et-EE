---
title: Luba Teams webinars
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793651"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="962a9-102">Luba Teams webinars</span><span class="sxs-lookup"><span data-stu-id="962a9-102">Enable Teams Webinars</span></span>

<span data-ttu-id="962a9-103">Webinars on vaikimisi lubatud.</span><span class="sxs-lookup"><span data-stu-id="962a9-103">Webinars are enabled by default.</span></span> <span data-ttu-id="962a9-104">PowerShelli käskude abil saate hallata, kes Teams ajastada ja Teams veebipõhiseid Teams registreerida.</span><span class="sxs-lookup"><span data-stu-id="962a9-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="962a9-105">Kõik kasutajad, kes saavad koosolekut luua, saavad luua ka veebisenarkoosoleku.</span><span class="sxs-lookup"><span data-stu-id="962a9-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="962a9-106">Kui soovite hallata seda, kes saab Teams ajastada, kasutage funktsiooni *AllowMeetingRegistration*.</span><span class="sxs-lookup"><span data-stu-id="962a9-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="962a9-107">Vaikimisi on *WhoCanRegister* lubatud ja selle väärtuseks on **seatud Kõik**.</span><span class="sxs-lookup"><span data-stu-id="962a9-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="962a9-108">Kui soovite koosoleku registreerimise välja lülitada, määrake *allowMeetingRegistration väärtuseks* **False (Väär).**</span><span class="sxs-lookup"><span data-stu-id="962a9-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="962a9-109">Nende sätete muutmiseks peate installima [Teams PowerShelli.](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="962a9-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="962a9-110">Lisaks jõustatakse koosolekupoliitikad Teams webinars.</span><span class="sxs-lookup"><span data-stu-id="962a9-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="962a9-111">Näiteks kui anonüümne liitumine on koosolekusätetes välja lülitatud, ei saa anonüümsed kasutajad veebiseinaritega liituda.</span><span class="sxs-lookup"><span data-stu-id="962a9-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="962a9-112">Lisateavet selle kohta, kes saab veebiseinarite jaoks registreeruda, leiate teemast [Webinarsi kasutajaks registreerujate konfigureerimine.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)</span><span class="sxs-lookup"><span data-stu-id="962a9-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="962a9-113">Lisateavet Microsofti loendite sätete kohta leiate teemast [Microsofti loendite sätete juhtimine.](/sharepoint/control-lists)</span><span class="sxs-lookup"><span data-stu-id="962a9-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>