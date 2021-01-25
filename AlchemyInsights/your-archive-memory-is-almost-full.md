---
title: Teie arhiivi postkast on peaaegu täis
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974277"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="0bd50-102">Teie arhiivi postkast on peaaegu täis</span><span class="sxs-lookup"><span data-stu-id="0bd50-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="0bd50-103">Kui kasutaja saab hoiatuse; **Teie arhiivi postkast on peaaegu täis** või peate suurendama arhiivi postkasti mahtu, siin on mõned näpunäited.</span><span class="sxs-lookup"><span data-stu-id="0bd50-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="0bd50-104">Kui kasutajale on määratud Exchange Online ' i leping 1, üleminekuks **Exchange Online ' i** lepingule 2 litsentsi suurendamiseks 50 GB-st kuni 100GB.</span><span class="sxs-lookup"><span data-stu-id="0bd50-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="0bd50-105">Kui kasutaja on juba määratud ühte järgmistest: **Exchange Online ' i leping 2** või Exchange Online ' i leping 1 koos Exchange Online ' i arhiivimise lisandmooduliga, kasutage allolevaid juhiseid, et lubada automaatne laiendamine arhiivimine:.</span><span class="sxs-lookup"><span data-stu-id="0bd50-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="0bd50-106">[Ühenduse loomine Exchange Online PowerShelliga](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="0bd50-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="0bd50-107">Käivitage kasutaja jaoks järgmine unifiedgroup.  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="0bd50-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="0bd50-108">Kasutajale lubatud kinnitamiseks käivitage järgmine unifiedgroup.  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="0bd50-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="0bd50-109">Lisateavet leiate järgmistest teemadest.</span><span class="sxs-lookup"><span data-stu-id="0bd50-109">For more information see:</span></span>

- [<span data-ttu-id="0bd50-110"> Luba piiramatu arhiveerimine – administraatori spikker – Microsoft 365 nõuetele vastavus | Microsoft docs</span><span class="sxs-lookup"><span data-stu-id="0bd50-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="0bd50-111">Exchange Online ' i limiidid – teenuste kirjeldused | Microsoft docs</span><span class="sxs-lookup"><span data-stu-id="0bd50-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="0bd50-112">Üleminek mõnele muule äriplaanile | Microsoft docs</span><span class="sxs-lookup"><span data-stu-id="0bd50-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

