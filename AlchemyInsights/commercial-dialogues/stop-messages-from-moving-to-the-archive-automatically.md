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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746327"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="b7598-102">Sõnumite automaatse teisaldamise takistamine automaatselt arhiivi</span><span class="sxs-lookup"><span data-stu-id="b7598-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="b7598-103">Säilituspoliitika kasutamise korral saate muuta selle poliitika säilituse vanust, et takistada sõnumite automaatset arhiivimist.</span><span class="sxs-lookup"><span data-stu-id="b7598-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="b7598-104">Tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="b7598-104">Here's how:</span></span>

1. <span data-ttu-id="b7598-105">Valige [Exchange ' i administreerimiskeskuses](https://go.microsoft.com/fwlink/?linkid=2059104) **vastavuse halduse**  >  **säilituse sildid**.</span><span class="sxs-lookup"><span data-stu-id="b7598-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="b7598-106">Otsige üles oma liigutused, et arhiivida säilituse silt.</span><span class="sxs-lookup"><span data-stu-id="b7598-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="b7598-107">Muutke säilituse perioodi (arhiivi periood), et **mitte kunagi** takistada üksuste automaatset arhiivimist säilituspoliitika abil.</span><span class="sxs-lookup"><span data-stu-id="b7598-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="b7598-108">See muudab kõigi postkastide arhiivimise sätteid, millele on rakendatud selle säilituse silt.</span><span class="sxs-lookup"><span data-stu-id="b7598-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
