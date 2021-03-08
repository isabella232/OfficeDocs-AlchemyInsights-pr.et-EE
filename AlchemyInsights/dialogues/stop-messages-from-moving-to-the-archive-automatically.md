---
title: Sõnumite automaatse teisaldamise takistamine automaatselt arhiivi
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50525100"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="972c2-102">Sõnumite automaatse teisaldamise takistamine automaatselt arhiivi</span><span class="sxs-lookup"><span data-stu-id="972c2-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="972c2-103">Säilituspoliitika kasutamise korral saate muuta selle poliitika säilituse vanust, et takistada sõnumite automaatset arhiivimist.</span><span class="sxs-lookup"><span data-stu-id="972c2-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="972c2-104">Tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="972c2-104">Here's how:</span></span>

1. <span data-ttu-id="972c2-105">Valige [Exchange ' i administreerimiskeskuses](https://go.microsoft.com/fwlink/?linkid=2059104) **vastavuse halduse**  >  **säilituse sildid**.</span><span class="sxs-lookup"><span data-stu-id="972c2-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="972c2-106">Otsige üles oma liigutused, et arhiivida säilituse silt.</span><span class="sxs-lookup"><span data-stu-id="972c2-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="972c2-107">Muutke säilituse perioodi (arhiivi periood), et **mitte kunagi** takistada üksuste automaatset arhiivimist säilituspoliitika abil.</span><span class="sxs-lookup"><span data-stu-id="972c2-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="972c2-108">See muudab kõigi postkastide arhiivimise sätteid, millele on rakendatud selle säilituse silt.</span><span class="sxs-lookup"><span data-stu-id="972c2-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
