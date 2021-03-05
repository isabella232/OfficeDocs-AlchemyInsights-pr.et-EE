---
title: Kasutaja loodud meilisõnumite signatuuride blokeerimine
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481576"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="b11c2-102">Kasutaja loodud meilisõnumite signatuuride blokeerimine</span><span class="sxs-lookup"><span data-stu-id="b11c2-102">Block user-made email signatures</span></span>

<span data-ttu-id="b11c2-103">Järgmine lahendus kehtib ainult Outlooki veebirakenduses loodud meilisõnumite signatuuride korral.</span><span class="sxs-lookup"><span data-stu-id="b11c2-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="b11c2-104">Kui teil on asutusesisene Exchange ' i server, saate Outlooki rakenduses signatuure blokeerida.</span><span class="sxs-lookup"><span data-stu-id="b11c2-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="b11c2-105">**Valige halduskeskus**  >  **Exchange ' i** halduskeskus.</span><span class="sxs-lookup"><span data-stu-id="b11c2-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="b11c2-106">Valige   >  **Outlook Web Appi poliitikate** permissions.</span><span class="sxs-lookup"><span data-stu-id="b11c2-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="b11c2-107">Valige poliitika ja seejärel klõpsake selle redigeerimiseks ikooni pliiats.</span><span class="sxs-lookup"><span data-stu-id="b11c2-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="b11c2-108">Klõpsake nuppu **funktsioonide**  >  **rohkem suvandeid**.</span><span class="sxs-lookup"><span data-stu-id="b11c2-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="b11c2-109">Tühjendage jaotises **kasutaja töökogemus** ruut **Meilisõnumi signatuur** ja seejärel klõpsake nuppu **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="b11c2-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="b11c2-110">**Oluline.** Kui enne selle märkeruudu tühjendamist lisati allkiri, saab kasutaja seda endiselt kasutada.</span><span class="sxs-lookup"><span data-stu-id="b11c2-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="b11c2-111">Paluge neil see eemaldada.</span><span class="sxs-lookup"><span data-stu-id="b11c2-111">Ask them to remove it.</span></span>
