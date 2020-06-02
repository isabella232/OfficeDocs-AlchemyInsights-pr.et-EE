---
title: Säilituspoliitikad Exchange ' i halduskeskus ei tööta
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 3040365b9d686bcbcce60977ee9bdbbaffc70b24
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502603"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="632de-102">Säilituspoliitikad Exchange ' i halduskeskus</span><span class="sxs-lookup"><span data-stu-id="632de-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="632de-103">**Probleem:** Äsja loodud või värskendatud Säilituspoliitikad Exchange ' i halduskeskus ei kohaldata postkastid või üksused on teisaldatud arhiivi postkasti või kustutatud.</span><span class="sxs-lookup"><span data-stu-id="632de-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="632de-104">**Algpõhjuste:**</span><span class="sxs-lookup"><span data-stu-id="632de-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="632de-105">Põhjuseks võib olla see, et **hallatud Kaustaabimeest** pole kasutaja postkasti töödeldud.</span><span class="sxs-lookup"><span data-stu-id="632de-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="632de-106">Hallatud kaustade abimees proovib töödelda iga postkasti oma pilvepõhise organisatsiooni kord iga seitsme päeva järel.</span><span class="sxs-lookup"><span data-stu-id="632de-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="632de-107">Kui muudate säilitusmärgendit või rakendada mõnda muud säilituspoliitika postkasti, saate oodata, kuni hallatav kaust aitab töötleb postkasti või käivitage cmdleti Start-ManagedFolderAssistant käivitada hallatav kaust abimehe töödelda konkreetse postkasti.</span><span class="sxs-lookup"><span data-stu-id="632de-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="632de-108">Selle cmdlet-käsu käitamine on kasulik säilituspoliitika või säilitusmärgendi sätete testimiseks või tõrkeotsinguks.</span><span class="sxs-lookup"><span data-stu-id="632de-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="632de-109">Lisateabe saamiseks külastage [hallatava kausta abimehe käivitamine](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="632de-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="632de-110">**Lahendus:** Käivitage järgmine käsk käivitada hallatav kaust Assistant konkreetse postkasti:</span><span class="sxs-lookup"><span data-stu-id="632de-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="632de-111">See võib ilmneda ka siis, kui **Retentionhold** on **lubatud** postkasti.</span><span class="sxs-lookup"><span data-stu-id="632de-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="632de-112">Kui postkast on paigutatud RetentionHold, säilituspoliitika postkasti ei töödelda selle aja jooksul.</span><span class="sxs-lookup"><span data-stu-id="632de-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="632de-113">Rohkem teavet kohta retentionhold säte vt: [postkasti säilitamise hoidke](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="632de-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="632de-114">**Lahendus:**</span><span class="sxs-lookup"><span data-stu-id="632de-114">**Solution:**</span></span>
    
  - <span data-ttu-id="632de-115">Kontrollige oleku RetentionHold kindla postkasti [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="632de-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="632de-116">Käivitage järgmine käsk **keelata** retentionhold konkreetse postkasti:</span><span class="sxs-lookup"><span data-stu-id="632de-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="632de-117">Nüüd käivitage hallatav kausta abimees uuesti:</span><span class="sxs-lookup"><span data-stu-id="632de-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="632de-118">**Märkus:** Kui postkast on väiksem kui 10 MB, hallatav kaust Assistant ei töötle automaatselt postkasti.</span><span class="sxs-lookup"><span data-stu-id="632de-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="632de-119">Exchange ' i halduskeskus säilituspoliitika kohta lisateabe saamiseks vaadake:</span><span class="sxs-lookup"><span data-stu-id="632de-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="632de-120">Säilitussildid ja Säilituspoliitikad</span><span class="sxs-lookup"><span data-stu-id="632de-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="632de-121">Säilituspoliitika rakendamine postkastidele</span><span class="sxs-lookup"><span data-stu-id="632de-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="632de-122">Säilitussiltide lisamine või eemaldamine</span><span class="sxs-lookup"><span data-stu-id="632de-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="632de-123">Kuidas tuvastada tüüpi hoidke postkasti</span><span class="sxs-lookup"><span data-stu-id="632de-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
