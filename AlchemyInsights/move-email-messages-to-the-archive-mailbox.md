---
title: Meilisõnumite ümberpaigutamine arhiivi postkasti
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799776"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="9c93b-102">Meilisõnumite saatmine arhiivi postkasti</span><span class="sxs-lookup"><span data-stu-id="9c93b-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="9c93b-103">Kui soovite, et me käivitaks allpool nimetatud sätete automatiseeritud kontrollimised, valige nupp tagasi <--selle lehe ülaosas ja seejärel sisestage selle kasutaja meiliaadress, kellel on probleeme meilisõnumite teisaldamisega arhiivi postkasti.</span><span class="sxs-lookup"><span data-stu-id="9c93b-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="9c93b-104">Veenduge, et **arhiivi postkast** oleks lubatud.</span><span class="sxs-lookup"><span data-stu-id="9c93b-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="9c93b-105">Kui seda ei ole, kasutage arhiivi postkasti lubamiseks [selles artiklis](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) toodud juhiseid.</span><span class="sxs-lookup"><span data-stu-id="9c93b-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="9c93b-106">Kui soovite arhiivi postkasti automaatselt arhiivida, **peab toimingu arhiivimiseks käsuga arhiivimine** olema seatud **automaatselt rakendama kogu postkasti (vaike) sildile**.</span><span class="sxs-lookup"><span data-stu-id="9c93b-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="9c93b-107">Selle toimingu abil saate luua sildi: [arhiivi vaikevormingu](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="9c93b-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="9c93b-108">Järgmisena lisage **arhiivi** silt oma säilituspoliitika.</span><span class="sxs-lookup"><span data-stu-id="9c93b-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="9c93b-109">Valige Exchange ' i halduskeskus > **säilituspoliitika** , et lisada poliitikasse > **salvestatav nupp Salvesta** **arhiivi** .</span><span class="sxs-lookup"><span data-stu-id="9c93b-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="9c93b-110">Nüüd [Määra säilituspoliitika](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) konkreetse kasutaja postkasti.</span><span class="sxs-lookup"><span data-stu-id="9c93b-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="9c93b-111">Sama poliitika rakendub nii **alg** -kui ka **arhiivi** postkastile.</span><span class="sxs-lookup"><span data-stu-id="9c93b-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="9c93b-112">Võimalik, et hallatava kausta assistent (MFA) peab käivitama ja rakendama kasutaja postkastile uusi sätteid.</span><span class="sxs-lookup"><span data-stu-id="9c93b-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="9c93b-113">Kindla postkasti hallatava kausta abilise käivitamiseks käivitage järgmine käsk, [ühendades selle ekso PowerShelliga](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) .</span><span class="sxs-lookup"><span data-stu-id="9c93b-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="9c93b-114">Start-ManagedFolderAssistant – identiteet <name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="9c93b-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="9c93b-115">Lisateavet arhiivimise poliitika häälestamise kohta leiate teemast [postkastide arhiivimise ja kustutamise poliitika häälestamine](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="9c93b-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  