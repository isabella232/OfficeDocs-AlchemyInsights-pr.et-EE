---
title: Teisalda e-kirjad arhiivi postkasti
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822158"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="5b9e2-102">Teisalda e-posti arhiivi postkasti</span><span class="sxs-lookup"><span data-stu-id="5b9e2-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="5b9e2-103">Veenduge, et **arhiivi postkast** on lubatud.</span><span class="sxs-lookup"><span data-stu-id="5b9e2-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="5b9e2-104">Kui ei, kasutage [selle artikli](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) juhiseid arhiivi postkasti lubamiseks.</span><span class="sxs-lookup"><span data-stu-id="5b9e2-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="5b9e2-105">Sõnumite automaatseks arhiivimiseks arhiivi postkasti, tuleb seada säilitamise silt koos **Teisalda arhiivi** toiming **automaatselt rakendada kogu postkasti (vaikimisi) silt**.</span><span class="sxs-lookup"><span data-stu-id="5b9e2-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="5b9e2-106">Sildi loomiseks kasutage siin olevaid juhiseid: [Arhiiv vaikimisi silt](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="5b9e2-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="5b9e2-107">Järgmisena lisage oma säilituspoliitikale **arhiivi** silt.</span><span class="sxs-lookup"><span data-stu-id="5b9e2-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="5b9e2-108">Exchange ' i halduskeskus, valige **säilituspoliitikad** > lisa **Arhiiv arhiivi sildi** poliitika > **salvestada**.</span><span class="sxs-lookup"><span data-stu-id="5b9e2-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="5b9e2-109">Nüüd [määrata säilituspoliitika](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) konkreetse kasutaja postkasti.</span><span class="sxs-lookup"><span data-stu-id="5b9e2-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="5b9e2-110">Sama poliitika rakendatakse nii **põhi** -kui ka **arhiivi** postkasti.</span><span class="sxs-lookup"><span data-stu-id="5b9e2-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="5b9e2-111">Võib osutuda vajalikuks sundida hallatav kaustade abimees (MFA) käivitada ja rakendada uusi sätteid kasutaja postkasti.</span><span class="sxs-lookup"><span data-stu-id="5b9e2-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="5b9e2-112">Käivitage järgmine käsk [ühendatud EXO PowerShelli](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) käivitada hallatav kaust Assistant konkreetse postkasti:</span><span class="sxs-lookup"><span data-stu-id="5b9e2-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="5b9e2-113">Start-ManagedFolderAssistant-identiteet<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="5b9e2-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="5b9e2-114">Lisateavet arhiivipoliitika seadistamise kohta leiate jaotisest [arhiivi-ja kustutuspoliitika häälestamine postkastide jaoks](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="5b9e2-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  