---
title: Ühenduste poliitika parandamine
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
- "9000760"
- "7391"
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694170"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="00083-102">Ühenduste poliitika parandamine</span><span class="sxs-lookup"><span data-stu-id="00083-102">Fix connection policy</span></span>

<span data-ttu-id="00083-103">Meilisõnum oli märgitud turvaliseks ja toimetatakse kasutaja sisendkausta, kuna saatmise IP-aadress oli märgitud turvaliseks filtri poliitikas.</span><span class="sxs-lookup"><span data-stu-id="00083-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="00083-104">Poliitika läbivaatamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="00083-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="00083-105">Minge [Office 365 turbe & nõuetele vastavuse keskusse](https://go.microsoft.com/fwlink/p/?linkid=2077143)ja seejärel valige **ohustatud halduse**  >  **poliitika**  >  [anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="00083-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="00083-106">Valige vahekaardil **kohandatud** **filtri poliitika** ja seejärel valige **Redigeeri poliitikat**.</span><span class="sxs-lookup"><span data-stu-id="00083-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="00083-107">Vaadake üle **IP-lubatute** loend.</span><span class="sxs-lookup"><span data-stu-id="00083-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="00083-108">Vaadake, kas **turvaline loend** on lubatud.</span><span class="sxs-lookup"><span data-stu-id="00083-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="00083-109">Microsoft tellib usaldusväärsete saatjate kolmanda osapoole allikaid.</span><span class="sxs-lookup"><span data-stu-id="00083-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="00083-110">Kui **turvaline loend** on lubatud, pole need usaldusväärsed saatjad ekslikult rämpspostina märgitud.</span><span class="sxs-lookup"><span data-stu-id="00083-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="00083-111">Soovitan valida selle suvandi, sest see vähendab valede positiivsete (hea meili, mis on klassifitseeritud rämpspostiks) arvu.</span><span class="sxs-lookup"><span data-stu-id="00083-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
