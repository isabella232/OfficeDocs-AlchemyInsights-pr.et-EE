---
title: Microsoft Defenderi Office 365 turvaliste manuste poliitikate näide
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
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745991"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="16c6c-102">Microsoft Defenderi Office 365 turvaliste manuste poliitikate näide</span><span class="sxs-lookup"><span data-stu-id="16c6c-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="16c6c-103">Need sätted võimaldavad poliitika, mis *ei sisalda viivitusi* , mis saadab sõnumeid kohe ja seejärel manustab manused pärast skannimist uuesti.</span><span class="sxs-lookup"><span data-stu-id="16c6c-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="16c6c-104">**Nimi**: viivitused puuduvad</span><span class="sxs-lookup"><span data-stu-id="16c6c-104">**Name**: No delays</span></span>
- <span data-ttu-id="16c6c-105">**Kirjeldus**: toimetab sõnumid kohe kohale ja manustab manused pärast skannimist uuesti.</span><span class="sxs-lookup"><span data-stu-id="16c6c-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="16c6c-106">**Vastus**: valige **dünaamiline kohaletoimetamise** suvand.</span><span class="sxs-lookup"><span data-stu-id="16c6c-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="16c6c-107">Lisateavet leiate teemast [dünaamilised tarned turvaliste manuste poliitikas](https://go.microsoft.com/fwlink/?linkid=2092328).</span><span class="sxs-lookup"><span data-stu-id="16c6c-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="16c6c-108">**Ümbersuunamise** jaotis: valige **ümbersuunamise lubamise** suvand ja seejärel sisestage oma Microsoft 365 Global Administratori, administraatori või turbe analüüsi meiliaadress, kes uurib pahatahtlikke manuseid.</span><span class="sxs-lookup"><span data-stu-id="16c6c-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="16c6c-109">Jaotises **rakendatav** : valige **adressaadi Domeen** ja seejärel valige oma domeen.</span><span class="sxs-lookup"><span data-stu-id="16c6c-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="16c6c-110">Valige **Lisa** ja seejärel klõpsake **nuppu OK**.</span><span class="sxs-lookup"><span data-stu-id="16c6c-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="16c6c-111">Kui olete lõpetanud, valige **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="16c6c-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="16c6c-112">Lisateavet leiate teemast [turvaliste manuste kuvamine rakenduses Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span><span class="sxs-lookup"><span data-stu-id="16c6c-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>
