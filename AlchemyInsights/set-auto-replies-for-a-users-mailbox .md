---
title: Kasutaja postkasti automaatvastuste määramine
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
ms.openlocfilehash: e3cc01298c10fd3ba21327a7fb5cc5396d0ad74d
ms.sourcegitcommit: 23e5b94f1758bfe202008384e300b81816975375
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/14/2020
ms.locfileid: "43506456"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="7b458-102">Kasutaja postkasti automaatvastuste määramine</span><span class="sxs-lookup"><span data-stu-id="7b458-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="7b458-103">**1. meetod**</span><span class="sxs-lookup"><span data-stu-id="7b458-103">**Method 1**</span></span>

1. <span data-ttu-id="7b458-104">Logige sisse Office 365 portaali.</span><span class="sxs-lookup"><span data-stu-id="7b458-104">Sign in to the Office 365 portal.</span></span>

2. <span data-ttu-id="7b458-105">Avage suvand **Kasutajad > Aktiivsed kasutajad** (või **Rühmad > Ühispostkastid**, kui määrate selle ühispostkastile).</span><span class="sxs-lookup"><span data-stu-id="7b458-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="7b458-106">Valige kasutaja, kellel on Microsoft Exchange’i postkast.</span><span class="sxs-lookup"><span data-stu-id="7b458-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="7b458-107">Avage parempoolses hüpikmenüüd **Meilisätted > Automaatvastused** (kui see on ühispostkast, klõpsake lihtsalt hüpikmenüüs suvandit **Automaatvastused**).</span><span class="sxs-lookup"><span data-stu-id="7b458-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="7b458-108">**2. meetod**</span><span class="sxs-lookup"><span data-stu-id="7b458-108">**Method 2**</span></span>

1. <span data-ttu-id="7b458-109">Logige administraatori identimisteavet kasutades sisse Office 365 haldusportaali.</span><span class="sxs-lookup"><span data-stu-id="7b458-109">Sign in to the Office 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="7b458-110">Laiendage suvandit **Halduskeskused** ja seejärel klõpsake suvandit **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="7b458-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="7b458-111">Klõpsake paremas ülanurgas olevat pilti, klõpsake suvandit **Teine kasutaja** ja seejärel valige kasutaja postkast, mida soovite muuta.</span><span class="sxs-lookup"><span data-stu-id="7b458-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="7b458-112">Valige vasakus servas valik **Suvandid**, klõpsake suvandit **Meilide korraldamine** ja klõpsake seejärel suvandit **Automaatvastused.**</span><span class="sxs-lookup"><span data-stu-id="7b458-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="7b458-113">**3. meetod**</span><span class="sxs-lookup"><span data-stu-id="7b458-113">**Method 3**</span></span>

<span data-ttu-id="7b458-114">Käivitage Exchange Online PowerShellis järgmine cmdlet-käsk:</span><span class="sxs-lookup"><span data-stu-id="7b458-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="7b458-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="7b458-115">PowerShellCopy</span></span>

    Set-MailboxAutoReplyConfiguration

<span data-ttu-id="7b458-116">Selle cmdlet-käsu kohta leiate lisateavet artiklist [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="7b458-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
