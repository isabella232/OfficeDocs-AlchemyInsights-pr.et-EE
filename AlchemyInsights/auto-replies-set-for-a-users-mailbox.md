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
ms.openlocfilehash: 4ffe8d77dad7db5fd5806fe879cf4934e5ca7c4a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/23/2020
ms.locfileid: "43788878"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="2220e-102">Kasutaja postkasti automaatvastuste määramine</span><span class="sxs-lookup"><span data-stu-id="2220e-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="2220e-103">**1. meetod**</span><span class="sxs-lookup"><span data-stu-id="2220e-103">**Method 1**</span></span>

1. <span data-ttu-id="2220e-104">Logige sisse Microsoft 365 portaali.</span><span class="sxs-lookup"><span data-stu-id="2220e-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="2220e-105">Avage suvand **Kasutajad > Aktiivsed kasutajad** (või **Rühmad > Ühispostkastid**, kui määrate selle ühispostkastile).</span><span class="sxs-lookup"><span data-stu-id="2220e-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="2220e-106">Valige kasutaja, kellel on Microsoft Exchange’i postkast.</span><span class="sxs-lookup"><span data-stu-id="2220e-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="2220e-107">Avage parempoolses hüpikmenüüd **Meilisätted > Automaatvastused** (kui see on ühispostkast, klõpsake lihtsalt hüpikmenüüs suvandit **Automaatvastused**).</span><span class="sxs-lookup"><span data-stu-id="2220e-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="2220e-108">**2. meetod**</span><span class="sxs-lookup"><span data-stu-id="2220e-108">**Method 2**</span></span>

1. <span data-ttu-id="2220e-109">Logige administraatori identimisteavet kasutades sisse Microsoft 365 haldusportaali.</span><span class="sxs-lookup"><span data-stu-id="2220e-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="2220e-110">Laiendage suvandit **Halduskeskused** ja seejärel klõpsake suvandit **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="2220e-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="2220e-111">Klõpsake paremas ülanurgas olevat pilti, klõpsake suvandit **Teine kasutaja** ja seejärel valige kasutaja postkast, mida soovite muuta.</span><span class="sxs-lookup"><span data-stu-id="2220e-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="2220e-112">Valige vasakus servas valik **Suvandid**, klõpsake suvandit **Meilide korraldamine** ja klõpsake seejärel suvandit **Automaatvastused.**</span><span class="sxs-lookup"><span data-stu-id="2220e-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="2220e-113">**3. meetod**</span><span class="sxs-lookup"><span data-stu-id="2220e-113">**Method 3**</span></span>

<span data-ttu-id="2220e-114">Käivitage Exchange Online PowerShellis järgmine cmdlet-käsk:</span><span class="sxs-lookup"><span data-stu-id="2220e-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="2220e-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="2220e-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="2220e-116">Selle cmdlet-käsu kohta leiate lisateavet artiklist [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="2220e-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
