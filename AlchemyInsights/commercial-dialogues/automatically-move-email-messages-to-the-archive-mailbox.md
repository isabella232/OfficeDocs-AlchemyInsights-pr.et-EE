---
title: Meilisõnumite automaatne ümberpaigutamine arhiivi postkasti
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
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746046"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="98dfb-102">Meilisõnumite automaatne ümberpaigutamine arhiivi postkasti</span><span class="sxs-lookup"><span data-stu-id="98dfb-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="98dfb-103">Siin on juhised selle kohta, kuidas häälestada poliitika kasutaja vana meili arhiivi postkasti automaatselt üle viima.</span><span class="sxs-lookup"><span data-stu-id="98dfb-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="98dfb-104">Valige [**turbe & nõuetele vastavuse**](https://go.microsoft.com/fwlink/p/?linkid=2077143)  >  **andmete haldamise**  >  **arhiivi** , et kontrollida, kas arhiivi postkast on kasutaja jaoks lubatud.</span><span class="sxs-lookup"><span data-stu-id="98dfb-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="98dfb-105">Kui pole, klõpsake väljal hoiatus nuppu **Luba** ja siis nuppu **Jah** .</span><span class="sxs-lookup"><span data-stu-id="98dfb-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="98dfb-106">Avage [**Exchange ' i halduskeskus > nõuetele vastavuse haldus > säilituse sildid**](https://go.microsoft.com/fwlink/?linkid=2059104).</span><span class="sxs-lookup"><span data-stu-id="98dfb-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="98dfb-107">Valige ikoon + ja seejärel valige nupp **Rakenda automaatselt tervele postkastile**.</span><span class="sxs-lookup"><span data-stu-id="98dfb-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="98dfb-108">Määrake säilituse sildile nimi ja valige käsk **VII arhiivi**.</span><span class="sxs-lookup"><span data-stu-id="98dfb-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="98dfb-109">Sisestage ooteaeg soovitud aeg (nt 90 päeva).</span><span class="sxs-lookup"><span data-stu-id="98dfb-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="98dfb-110">Klõpsake nuppu **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="98dfb-110">Click **Save**.</span></span>
5. <span data-ttu-id="98dfb-111">Nüüd looge säilituspoliitika: valige **säilituspoliitika**, valige uue poliitika lisamiseks ikoon.</span><span class="sxs-lookup"><span data-stu-id="98dfb-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="98dfb-112">Määrake säilituspoliitika nimi, seejärel klõpsake ja liikuge, et leida ja lisada äsja loodud säilituse silt.</span><span class="sxs-lookup"><span data-stu-id="98dfb-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="98dfb-113">Klõpsake nuppu **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="98dfb-113">Click **Save**.</span></span>
7. <span data-ttu-id="98dfb-114">Lõpuks rakendage säilituspoliitika kasutaja postkastile: endiselt Exchange ' i administreerimiskeskuses Avage **adressaadi**  >  **postkastid**.</span><span class="sxs-lookup"><span data-stu-id="98dfb-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="98dfb-115">Valige kõik kasutajad, kellele soovite poliitika rakendada, ja seejärel valige käsk **Redigeeri** (pliiatsi ikoon).</span><span class="sxs-lookup"><span data-stu-id="98dfb-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="98dfb-116">Klõpsake dialoogiboksis nuppu **postkasti funktsioonid**.</span><span class="sxs-lookup"><span data-stu-id="98dfb-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="98dfb-117">Rakendage jaotises **säilituspoliitika** selle poliitika, mille äsja lõite > **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="98dfb-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="98dfb-118">Juhised poliitika rakendamiseks kõigile kasutajatele leiate teemast [säilituspoliitika rakendamine postkastidele](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span><span class="sxs-lookup"><span data-stu-id="98dfb-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
