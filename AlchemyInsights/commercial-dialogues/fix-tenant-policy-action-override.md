---
title: Rentniku poliitika lahendamine (toimingu alistamine)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745879"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="38813-102">Rentniku poliitika lahendamine (toimingu alistamine)</span><span class="sxs-lookup"><span data-stu-id="38813-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="38813-103">See sõnum mõjutas teie rentniku rämpsposti poliitikat.</span><span class="sxs-lookup"><span data-stu-id="38813-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="38813-104">Poliitika läbivaatamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="38813-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="38813-105">Minge [Office 365 turbe & nõuetele vastavuse keskusse](https://go.microsoft.com/fwlink/p/?linkid=2077143)ja seejärel valige **ohustatud halduse**  >  **poliitika**  >  [anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="38813-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="38813-106">Kontrollige, kas **poliitika allikas** viitab järgmistele teemale:  **Add-Xheader/ModifySubject/ümbersuunamine/DELETE/ei toimingu/Salakoopia sõnum**</span><span class="sxs-lookup"><span data-stu-id="38813-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="38813-107">Kui see on nii, siis kontrollige, kas vahekaardil **kohandatud** kuvatakse sõnumiga mõjutatud poliitika sätted.</span><span class="sxs-lookup"><span data-stu-id="38813-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="38813-108">On võimalik, et kõik Exchange Online ' i kaitstud kliendid rakendasid sõnumile **normi** .</span><span class="sxs-lookup"><span data-stu-id="38813-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="38813-109">Lisateavet rämpsmeili filtri poliitikate konfigureerimise kohta leiate teemast [rämpsmeili filtri poliitikate konfigureerimine](https://go.microsoft.com/fwlink/?linkid=2101431).</span><span class="sxs-lookup"><span data-stu-id="38813-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
