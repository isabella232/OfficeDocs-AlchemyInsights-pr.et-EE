---
title: Postkasti automaatvastuste määramine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: aeeb2e1e76fe602d2767b422797452fd1155fdd5
ms.sourcegitcommit: fdfd41c2bfb2d45003b3906e6469377384a91cb5
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2020
ms.locfileid: "43509490"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="c47a2-102">Kasutaja postkasti automaatvastuste määramine</span><span class="sxs-lookup"><span data-stu-id="c47a2-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="c47a2-103">**1. meetod**</span><span class="sxs-lookup"><span data-stu-id="c47a2-103">**Method 1**</span></span>

1. <span data-ttu-id="c47a2-104">Logige sisse Office 365 portaali.</span><span class="sxs-lookup"><span data-stu-id="c47a2-104">Sign in to the Office 365 portal.</span></span>

2. <span data-ttu-id="c47a2-105">Avage suvand **Kasutajad > Aktiivsed kasutajad** (või **Rühmad > Ühispostkastid**, kui määrate selle ühispostkastile).</span><span class="sxs-lookup"><span data-stu-id="c47a2-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="c47a2-106">Valige kasutaja, kellel on Microsoft Exchange’i postkast.</span><span class="sxs-lookup"><span data-stu-id="c47a2-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="c47a2-107">Avage parempoolses hüpikmenüüd **Meilisätted > Automaatvastused** (kui see on ühispostkast, klõpsake lihtsalt hüpikmenüüs suvandit **Automaatvastused**).</span><span class="sxs-lookup"><span data-stu-id="c47a2-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="c47a2-108">**2. meetod**</span><span class="sxs-lookup"><span data-stu-id="c47a2-108">**Method 2**</span></span>

1. <span data-ttu-id="c47a2-109">Logige administraatori identimisteavet kasutades sisse Office 365 haldusportaali.</span><span class="sxs-lookup"><span data-stu-id="c47a2-109">Sign in to the Office 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="c47a2-110">Laiendage suvandit **Halduskeskused** ja seejärel klõpsake suvandit **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="c47a2-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="c47a2-111">Klõpsake paremas ülanurgas olevat pilti, klõpsake suvandit **Teine kasutaja** ja seejärel valige kasutaja postkast, mida soovite muuta.</span><span class="sxs-lookup"><span data-stu-id="c47a2-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="c47a2-112">Valige vasakus servas valik **Suvandid**, klõpsake suvandit **Meilide korraldamine** ja klõpsake seejärel suvandit **Automaatvastused.**</span><span class="sxs-lookup"><span data-stu-id="c47a2-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="c47a2-113">**3. meetod**</span><span class="sxs-lookup"><span data-stu-id="c47a2-113">**Method 3**</span></span>

<span data-ttu-id="c47a2-114">Käivitage Exchange Online PowerShellis järgmine cmdlet-käsk:</span><span class="sxs-lookup"><span data-stu-id="c47a2-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="c47a2-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="c47a2-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="c47a2-116">Selle cmdlet-käsu kohta leiate lisateavet artiklist [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="c47a2-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
