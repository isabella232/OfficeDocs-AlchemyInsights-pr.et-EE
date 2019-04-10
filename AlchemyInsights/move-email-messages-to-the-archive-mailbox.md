---
title: Liikumine e-kirju arhiivi postkasti
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 37f256ef31402f5139fdd7c2af8f3a6ca9dc3525
ms.sourcegitcommit: 228c986911ecf73217116a5d1fdcd2e89362774e
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/09/2019
ms.locfileid: "31747199"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="3f5b8-102">Tõsta meil arhiivi postkasti</span><span class="sxs-lookup"><span data-stu-id="3f5b8-102">Move email to the archive mailbox</span></span>
 
1. <span data-ttu-id="3f5b8-103">Kinnitada, et on **arhiivi postkasti** on aktiivne.</span><span class="sxs-lookup"><span data-stu-id="3f5b8-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="3f5b8-104">Kui ei, siis kasutage [käesoleva artikli](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) juhiseid arhiivi postkasti lubamine.</span><span class="sxs-lookup"><span data-stu-id="3f5b8-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="3f5b8-105">Sõnumite automaatselt arhiivipostkasti arhiveerimisel seadma säilitussilti **teisaldamiseni** meetmega taotletud **automaatselt kogu postkasti (vaikimisi) tag**.</span><span class="sxs-lookup"><span data-stu-id="3f5b8-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="3f5b8-106">Tehke siin luua tag: [tag arhiiv vaikimisi](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).</span><span class="sxs-lookup"><span data-stu-id="3f5b8-106">Use the steps here to create the tag: [Archive Default tag](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).</span></span>
    
3. <span data-ttu-id="3f5b8-107">Seejärel lisada sildi **Arhiiv** oma säilituspoliitika.</span><span class="sxs-lookup"><span data-stu-id="3f5b8-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="3f5b8-108">Valige Exchange'i halduskeskuse **Säilituspoliitikate** > lisada **tag arhiivi teisaldada** poliitika > **salvestada**.</span><span class="sxs-lookup"><span data-stu-id="3f5b8-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span> 
    
4. <span data-ttu-id="3f5b8-109">Nüüd [määrata säilituspoliitika](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) kindla kasutaja postkastiga.</span><span class="sxs-lookup"><span data-stu-id="3f5b8-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="3f5b8-110">Sedasama kohaldatakse ka **esmase** ja **arhiivipostkasti** .</span><span class="sxs-lookup"><span data-stu-id="3f5b8-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="3f5b8-111">Tuleb sundida õnnestus kausta abimehe (MFA) ja uued sätted rakenduvad kasutaja postkasti.</span><span class="sxs-lookup"><span data-stu-id="3f5b8-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="3f5b8-112">Käivitada samal ajal [ühendatud EKSO PowerShelli](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) alustada abiline konkreetsele postkastile järgmine käsk:</span><span class="sxs-lookup"><span data-stu-id="3f5b8-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="3f5b8-113">Arhiivipoliitika seadistamise kohta lisateabe saamiseks vaadake teemat [arhiivi ja kustutamise poliitika postkastide](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="3f5b8-113">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

