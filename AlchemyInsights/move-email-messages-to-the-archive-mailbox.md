---
title: Liikumine e-kirju arhiivi postkasti
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 41d6825b568263fb7b09066b65235aa348415bae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28286123"
---
<span data-ttu-id="0ba43-p101">Arhiivi postkasti üksuste arhiivimise probleeme. Veenduge, et olete sooritanud järgmised sammud:</span><span class="sxs-lookup"><span data-stu-id="0ba43-p101">Having problems archiving items to the Archive mailbox. Make sure you have performed the following steps:</span></span>
  
1. <span data-ttu-id="0ba43-p102">Kinnitada, et on **arhiivi postkasti** on aktiivne. Kui ei, siis kasutage [käesoleva artikli](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) juhiseid arhiivi postkasti lubamine.</span><span class="sxs-lookup"><span data-stu-id="0ba43-p102">Confirm that an **Archive mailbox** has been enabled. If not, use steps in [this article](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span> 
    
2. <span data-ttu-id="0ba43-106">Exchange'i halduskeskuse abil, valige **Säilitussiltide** alusel **Nõuetele vastavuse tagamine**, **Teisalda arhiivi** meetmega, mis sisaldab soovitud **Säilituseani** **säilitussildi** loomine.</span><span class="sxs-lookup"><span data-stu-id="0ba43-106">In the Exchange Admin Center, select **Retention Tags** under **Compliance Management**, create a **Retention tag** with the **Move to Archive** action containing the desired **Retention Age**.</span></span>
    
3. <span data-ttu-id="0ba43-107">Exchange'i halduskeskuse abil, valige **Säilituspoliitikad**, **Säilituspoliitika** loomine ja **Teisalda arhiivi** säilitussildi lisamine poliitika.</span><span class="sxs-lookup"><span data-stu-id="0ba43-107">In the Exchange Admin Center, select **Retention Policies**, create a **Retention Policy** and add your **Move to Archive** retention tag to that policy.</span></span> 
    
4. <span data-ttu-id="0ba43-p103">[Säilituspoliitika määrata](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) konkreetse kasutaja postkasti. Sedasama kohaldatakse ka **esmase** ja **arhiivipostkasti** .</span><span class="sxs-lookup"><span data-stu-id="0ba43-p103">[Assign the Retention Policy](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="0ba43-p104">Kasutaja postkasti peaks nüüd olema kaupade liigutamiseks arhiivipostkasti arhiivipoliitika. Tuleb sundida õnnestus kausta abimehe (MFA) ja uued sätted rakenduvad kasutaja postkasti. Käivitada samal ajal [ühendatud EKSO PowerShelli](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) alustada abiline konkreetsele postkastile järgmine käsk:</span><span class="sxs-lookup"><span data-stu-id="0ba43-p104">The user's mailbox should now have an Archive policy to move items to the Archive mailbox. It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox. Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="0ba43-113">Lisainfot arhiivipoliitika seadistamise kohta, vaadake teemat [arhiivi ja kustutamise poliitika postkastide](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="0ba43-113">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

