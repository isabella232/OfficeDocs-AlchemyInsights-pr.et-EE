---
title: Teamsi lubamine või keelamine IP video
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002537"
- "5617"
ms.openlocfilehash: cf2d67170f846db1d5d2f1ca8c8b50902e200e45
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670180"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="e334b-102">Teamsi lubamine või keelamine IP video</span><span class="sxs-lookup"><span data-stu-id="e334b-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="e334b-103">**Koosoleku poliitika muutmine või loomine**</span><span class="sxs-lookup"><span data-stu-id="e334b-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="e334b-104">Koosolekupoliitika muutmiseks või loomiseks avage **Microsoft teamsi halduskeskus > koosolekud > koosolekute poliitikad**.</span><span class="sxs-lookup"><span data-stu-id="e334b-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="e334b-105">Valige loendist poliitika või klõpsake nuppu **Lisa**.</span><span class="sxs-lookup"><span data-stu-id="e334b-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="e334b-106">Kui loote uut poliitikat, lisage nimi ja kirjeldus.</span><span class="sxs-lookup"><span data-stu-id="e334b-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="e334b-107">Nimi ei tohi sisaldada erimärke ega olla pikem kui 64 märki.</span><span class="sxs-lookup"><span data-stu-id="e334b-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="e334b-108">Valige soovitud sätted ja klõpsake siis nuppu **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="e334b-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="e334b-109">Oletame näiteks, et teil on palju kasutajaid ja soovite piirata nende koosolekul nõutud läbilaskevõime mahtu.</span><span class="sxs-lookup"><span data-stu-id="e334b-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="e334b-110">Sel juhul võiksite luua uue kohandatud poliitika nimega „Piiratud läbilaskevõime“ ja keelata järgmised sätted.</span><span class="sxs-lookup"><span data-stu-id="e334b-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="e334b-111">Jaotises **Heli ja video** tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="e334b-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="e334b-112">Lülitage välja säte „Luba pilve salvestamine“.</span><span class="sxs-lookup"><span data-stu-id="e334b-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="e334b-113">Lülitage välja säte „Luba IP-video“.</span><span class="sxs-lookup"><span data-stu-id="e334b-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="e334b-114">Seejärel määrake poliitika kasutajatele.</span><span class="sxs-lookup"><span data-stu-id="e334b-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="e334b-115">**Koosolekupoliitika määramine kasutajatele**</span><span class="sxs-lookup"><span data-stu-id="e334b-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="e334b-116">Microsoft Teamsi halduskeskuse vasakpoolsel navigeerimisribal valige **Kasutajad** ja klõpsake soovitud kasutajat.</span><span class="sxs-lookup"><span data-stu-id="e334b-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="e334b-117">Valige kasutaja, klõpsates kasutajanimest vasakul. Seejärel klõpsake käsku **Muuda sätteid**.</span><span class="sxs-lookup"><span data-stu-id="e334b-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="e334b-118">Valige jaotises **koosoleku poliitika**poliitika, mille soovite määrata, ja seejärel klõpsake nuppu **Rakenda**.</span><span class="sxs-lookup"><span data-stu-id="e334b-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="e334b-119">Lisateavet leiate teemast [koosolekute poliitikate haldamine töörühmades](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="e334b-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>
