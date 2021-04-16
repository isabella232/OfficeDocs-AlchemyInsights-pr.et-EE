---
title: Teamsi otseedastussündmuste kasutamise alustamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000208"
- "3436"
ms.openlocfilehash: a10f756fc69a7a135446d8d3bcec1f5e951627d8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811956"
---
# <a name="getting-started-with-teams-live-events"></a><span data-ttu-id="de912-102">Teamsi otseedastussündmuste kasutamise alustamine</span><span class="sxs-lookup"><span data-stu-id="de912-102">Getting started with Teams live events</span></span>

<span data-ttu-id="de912-103">Microsoft Teamsi otseedastussündmused on Teamsi koosolekute laiendus, mis võimaldab teil plaanida ja luua sündmuseid, mis edastatakse suurtele veebipublikutele.</span><span class="sxs-lookup"><span data-stu-id="de912-103">Microsoft Teams live events are an extension of Teams meetings that enable you to schedule and produce events that stream to large online audiences.</span></span>

<span data-ttu-id="de912-104">Otseedastussündmuse loomiseks on teil vaja järgnevat.</span><span class="sxs-lookup"><span data-stu-id="de912-104">To create a live event, you will need the following:</span></span>

- <span data-ttu-id="de912-105">Esmalt veenduge, et Teams otseedastussündmused on [saadaval teie riigis ja regioonis](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Mõnes riigis pole otseedastussündmused veel toetatud.</span><span class="sxs-lookup"><span data-stu-id="de912-105">First, confirm that Teams Live Events are [available in your Country and Region](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Live Events are not yet supported in some countries.</span></span>  <span data-ttu-id="de912-106">Kui olete määranud litsentsid ja poliitikad, kuid ei saa siiski Teams otseedastussündmust luua, olete tõenäoliselt riigis või regioonis, kus otseedastussündmused pole veel saadaval.</span><span class="sxs-lookup"><span data-stu-id="de912-106">If you’ve assigned licenses and set policies, but still cannot create a Teams Live Event, it is likely you are in a Country or Region where Live Events is not yet available.</span></span>

- <span data-ttu-id="de912-107">[Office 365 Enterprise E1, E3 või E5 litsents või Office 365 A3 või A5 litsents](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="de912-107">An [Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span></span> <span data-ttu-id="de912-108">**Märkus**: Teamsi kasutamise hiljutise suurenemise tõttu võib kasutajale Teamsi litsentsi määramiseks kuluda umbes 24 tundi, enne kui see on täielikult seadistatud.</span><span class="sxs-lookup"><span data-stu-id="de912-108">**Note**: Due to a recent increase in Teams usage, when you assign a Teams license to a user, it may take around 24 hours before they'll be fully set up.</span></span> <span data-ttu-id="de912-109">Seni ei saa te neile Teamsi poliitikaid määrata ja neil ei pruugi olla juurdepääsu mõnele Teamsi funktsioonile (nt helistamine ja helikonverents).</span><span class="sxs-lookup"><span data-stu-id="de912-109">Until then, you won't be able to assign Teams policies to them, and they might not have access to some Teams features like calling and audio conferencing.</span></span>

- <span data-ttu-id="de912-110">Luba [luua Microsoft Teamsi halduskeskuses otseedastussündmuseid](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span><span class="sxs-lookup"><span data-stu-id="de912-110">Permission to [create live events in Microsoft Teams admin center](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span></span>

- <span data-ttu-id="de912-111">Luba [luua sündmuseid rakenduses Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (välist leviedastuse rakendust või seadet kasutades loodud sündmuste jaoks).</span><span class="sxs-lookup"><span data-stu-id="de912-111">Permission to [create live events in Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (for events produced using an external broadcasting app or device).</span></span>

- <span data-ttu-id="de912-112">Organisatsiooni meeskonna täisliikme staatus (ei saa olla külaline ega mõne muu organisatsiooni liige).</span><span class="sxs-lookup"><span data-stu-id="de912-112">Full team membership in the org (can't be a guest or from another org).</span></span>
<span data-ttu-id="de912-113">Privaatkoosoleku plaanimine, ekraani jagamine ja IP-video ühiskasutus Teamsi koosoleku poliitikas sisse lülitatud.</span><span class="sxs-lookup"><span data-stu-id="de912-113">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

- <span data-ttu-id="de912-114">Teamsi otseedastussündmuste[head tavad](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42).</span><span class="sxs-lookup"><span data-stu-id="de912-114">[Best practices](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) for Teams Live Events.</span></span>

<span data-ttu-id="de912-115">Lisateavet vaadake teemast [Microsoft Teamsi otseedastussündmuste kasutamise alustamine](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span><span class="sxs-lookup"><span data-stu-id="de912-115">For more information, please see [Get started with Microsoft Teams live events](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span></span>