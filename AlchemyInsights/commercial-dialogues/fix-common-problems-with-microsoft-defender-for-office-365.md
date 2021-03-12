---
title: Microsoft Defenderi for Office 365 levinumate probleemide lahendamine
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
ms.openlocfilehash: 05fa518ece7ea40fd7b4cea57115d9cd60370b01
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746830"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a><span data-ttu-id="100d9-102">Microsoft Defenderi for Office 365 levinumate probleemide lahendamine</span><span class="sxs-lookup"><span data-stu-id="100d9-102">Fix common problems with Microsoft Defender for Office 365</span></span>

<span data-ttu-id="100d9-103">Siin on mõned lahendused levinud probleemidele Microsoft Defenderi Office 365 jaoks.</span><span class="sxs-lookup"><span data-stu-id="100d9-103">Here are some solutions to common problems with Microsoft Defender for Office 365:</span></span>

- <span data-ttu-id="100d9-104">**Sõnumi viivitus:** Kui teil on probleeme sõnumi kohaletoimetamisega, soovite kasutada turvaliste manuste poliitikas **dünaamilisi kohaletoimetamise** suvandeid.</span><span class="sxs-lookup"><span data-stu-id="100d9-104">**Message delay:** If you're experiencing issues where message delivery is delayed, you'll want to use the **Dynamic Delivery** options within your Safe Attachments policy.</span></span> <span data-ttu-id="100d9-105">Lisateavet leiate teemast [dünaamilised tarned turvaliste manuste poliitikas](https://go.microsoft.com/fwlink/?linkid=2094106).</span><span class="sxs-lookup"><span data-stu-id="100d9-105">To learn more, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2094106).</span></span>
- <span data-ttu-id="100d9-106">**Valede positiivsete või negatiivsete tulemite teatamine.** Teavitage sõnumit Microsoftile selle lingi kaudu: [Microsoft Defenderi tagasiside portaal](https://go.microsoft.com/fwlink/?linkid=2092835).</span><span class="sxs-lookup"><span data-stu-id="100d9-106">**Report false positive or negative results:** Report the message to Microsoft using this link: [Microsoft Defender Response Portal](https://go.microsoft.com/fwlink/?linkid=2092835).</span></span>
- <span data-ttu-id="100d9-107">**Turvaliste linkide kaitse lubamine.**</span><span class="sxs-lookup"><span data-stu-id="100d9-107">**Enable Safe Link protection:**</span></span>
    1. <span data-ttu-id="100d9-108">Logige sisse [Office 365 turbe & nõuetele vastavuse keskuses](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="100d9-108">Sign in to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
    2. <span data-ttu-id="100d9-109">Valige **ohustatud halduse**  >  **poliitika**  >  **Turvalised lingid.**</span><span class="sxs-lookup"><span data-stu-id="100d9-109">Go to **Threat Management** > **Policy** > **Safe Links.**</span></span>
    3. <span data-ttu-id="100d9-110">Avage poliitika, **mis rakendub kindlatele adressaatidele**, ja avage konfigureeritud poliitika.</span><span class="sxs-lookup"><span data-stu-id="100d9-110">Under **Policies that apply to specific recipients**, open the policy configured.</span></span>
    4. <span data-ttu-id="100d9-111">Valige jaotises **sätted** **organisatsioonis saadetud sõnumitele nupp Rakenda turvalised lingid**.</span><span class="sxs-lookup"><span data-stu-id="100d9-111">Under **Settings**, select **Apply safe links to messages sent within the organization**.</span></span>
