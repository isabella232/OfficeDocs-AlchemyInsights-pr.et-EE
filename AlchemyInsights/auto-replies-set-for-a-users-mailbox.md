---
title: Postkasti automaatvastuste määramine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 60af581e7fe508ab9644a53873bcd551b3aacff1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820930"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="97cd6-102">Kasutaja postkasti automaatvastuste määramine</span><span class="sxs-lookup"><span data-stu-id="97cd6-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="97cd6-103">**1. meetod**</span><span class="sxs-lookup"><span data-stu-id="97cd6-103">**Method 1**</span></span>

1. <span data-ttu-id="97cd6-104">Logige sisse Microsoft 365 portaali.</span><span class="sxs-lookup"><span data-stu-id="97cd6-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="97cd6-105">Avage suvand **Kasutajad > Aktiivsed kasutajad** (või **Rühmad > Ühispostkastid**, kui määrate selle ühispostkastile).</span><span class="sxs-lookup"><span data-stu-id="97cd6-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="97cd6-106">Valige kasutaja, kellel on Microsoft Exchange’i postkast.</span><span class="sxs-lookup"><span data-stu-id="97cd6-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="97cd6-107">Avage parempoolses hüpikmenüüd **Meilisätted > Automaatvastused** (kui see on ühispostkast, klõpsake lihtsalt hüpikmenüüs suvandit **Automaatvastused**).</span><span class="sxs-lookup"><span data-stu-id="97cd6-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="97cd6-108">**2. meetod**</span><span class="sxs-lookup"><span data-stu-id="97cd6-108">**Method 2**</span></span>

1. <span data-ttu-id="97cd6-109">Logige administraatori identimisteavet kasutades sisse Microsoft 365 haldusportaali.</span><span class="sxs-lookup"><span data-stu-id="97cd6-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="97cd6-110">Laiendage suvandit **Halduskeskused** ja seejärel klõpsake suvandit **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="97cd6-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="97cd6-111">Klõpsake paremas ülanurgas olevat pilti, klõpsake suvandit **Teine kasutaja** ja seejärel valige kasutaja postkast, mida soovite muuta.</span><span class="sxs-lookup"><span data-stu-id="97cd6-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="97cd6-112">Valige vasakus servas valik **Suvandid**, klõpsake suvandit **Meilide korraldamine** ja klõpsake seejärel suvandit **Automaatvastused.**</span><span class="sxs-lookup"><span data-stu-id="97cd6-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="97cd6-113">**3. meetod**</span><span class="sxs-lookup"><span data-stu-id="97cd6-113">**Method 3**</span></span>

<span data-ttu-id="97cd6-114">Käivitage Exchange Online PowerShellis järgmine cmdlet-käsk:</span><span class="sxs-lookup"><span data-stu-id="97cd6-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="97cd6-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="97cd6-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="97cd6-116">Selle cmdlet-käsu kohta leiate lisateavet artiklist [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="97cd6-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
