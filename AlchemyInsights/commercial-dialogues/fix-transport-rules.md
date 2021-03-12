---
title: Transpordi reeglite parandamine
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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746733"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="d0da2-102">Transpordi reeglite parandamine</span><span class="sxs-lookup"><span data-stu-id="d0da2-102">Fix transport rules</span></span>

<span data-ttu-id="d0da2-103">See sõnum mõjutas kohandatud meilivoo reeglit.</span><span class="sxs-lookup"><span data-stu-id="d0da2-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="d0da2-104">Täpse reegli läbivaatamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="d0da2-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="d0da2-105">Märkige tulemite esitamisel jaotises **Lisateave** üles **GUID** või **poliitika nimi**.</span><span class="sxs-lookup"><span data-stu-id="d0da2-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="d0da2-106">Käivitage Exchange Management shell.</span><span class="sxs-lookup"><span data-stu-id="d0da2-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="d0da2-107">Lisateavet leiate teemast [Exchange ' i halduse kesta avamine](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="d0da2-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="d0da2-108">Käivitage see käsk (GUID-i abil oma edastusest):  **Get-TransportRule-Identity "GUID" | FL \* kirjeldus**\*</span><span class="sxs-lookup"><span data-stu-id="d0da2-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="d0da2-109">Vaadake kirjeldus üle, et näha sõnumit mõjutanud konfigureeritud tingimusi.</span><span class="sxs-lookup"><span data-stu-id="d0da2-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="d0da2-110">Lisateavet leiate teemast [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span><span class="sxs-lookup"><span data-stu-id="d0da2-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
