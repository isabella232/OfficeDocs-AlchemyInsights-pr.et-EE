---
title: Exchange ' i administreerimiskeskuse poliitikate säilitamine ei tööta
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
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740506"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="a6c10-102">Säilituspoliitika Exchange ' i administreerimiskeskuses</span><span class="sxs-lookup"><span data-stu-id="a6c10-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="a6c10-103">Kui soovite, et me käivitaks allpool mainitud sätete automatiseeritud kontrolli, valige nupp tagasi <--selle lehe ülaosas ja seejärel sisestage selle kasutaja meiliaadress, kellel on säilituspoliitika probleeme.</span><span class="sxs-lookup"><span data-stu-id="a6c10-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="a6c10-104">**Probleem:** Exchange ' i administreerimiskeskuse äsja loodud või värskendatud säilituspoliitika ei rakendu postkastidele ega üksustele ei teisaldata arhiivi postkasti ega kustutatud.</span><span class="sxs-lookup"><span data-stu-id="a6c10-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="a6c10-105">**Juure põhjused.**</span><span class="sxs-lookup"><span data-stu-id="a6c10-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="a6c10-106">Selle põhjuseks võib olla, et **hallatud kaustade abiline** pole kasutaja postkasti töödelnud.</span><span class="sxs-lookup"><span data-stu-id="a6c10-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="a6c10-107">Hallatud kaustade assistent proovib töödelda iga teie pilvepõhise asutuse postkasti iga seitsme päeva järel.</span><span class="sxs-lookup"><span data-stu-id="a6c10-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="a6c10-108">Kui muudate säilituse silti või rakendate postkastile mõne muu säilituspoliitika, võite oodata, kuni hallatav kaust teie postkasti töötleb, või käivitage ManagedFolderAssistant cmdlet-käsk, et käivitada hallatavate kaustade abiline kindla postkasti töötlemiseks.</span><span class="sxs-lookup"><span data-stu-id="a6c10-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="a6c10-109">Selle cmdlet-käsu käivitamine on kasulik säilituspoliitika või säilituse siltide sätete katsetamiseks või tõrkeotsinguks.</span><span class="sxs-lookup"><span data-stu-id="a6c10-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="a6c10-110">Lisateavet leiate teemast [hallatava kausta abilise käivitamine](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="a6c10-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="a6c10-111">**Lahendus:** Hallatava kausta abilise käivitamiseks kindla postkasti korral käivitage järgmine käsk.</span><span class="sxs-lookup"><span data-stu-id="a6c10-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="a6c10-112">See võib ilmneda ka juhul, kui postkastis on **RetentionHold** **lubatud** .</span><span class="sxs-lookup"><span data-stu-id="a6c10-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="a6c10-113">Kui postkast on paigutatud RetentionHold, siis postkasti säilituspoliitika ei töödelda selle aja jooksul.</span><span class="sxs-lookup"><span data-stu-id="a6c10-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="a6c10-114">RetentionHold Informaton kohta leiate lisateavet järgmistest teemadest: [postkasti säilituse ootelepanek](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="a6c10-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="a6c10-115">**Lahendus**</span><span class="sxs-lookup"><span data-stu-id="a6c10-115">**Solution:**</span></span>
    
  - <span data-ttu-id="a6c10-116">Kontrollige, kas RetentionHold säte on kindlas postkastis, mis asub [ekso PowerShellis](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="a6c10-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="a6c10-117">RetentionHold **keelamiseks** kindlal postkastil käivitage järgmine käsk.</span><span class="sxs-lookup"><span data-stu-id="a6c10-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="a6c10-118">Käivitage uuesti hallatavate kaustade abiline.</span><span class="sxs-lookup"><span data-stu-id="a6c10-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="a6c10-119">**Märkus:** Kui postkast on väiksem kui 10 MB, siis ei töötle hallatud kaustade assistent postkasti automaatselt.</span><span class="sxs-lookup"><span data-stu-id="a6c10-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="a6c10-120">Lisateavet Exchange ' i administreerimiskeskuse poliitikate kohta leiate järgmistest teemadest.</span><span class="sxs-lookup"><span data-stu-id="a6c10-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="a6c10-121">Säilituse siltide ja säilituspoliitika põhimõtted</span><span class="sxs-lookup"><span data-stu-id="a6c10-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="a6c10-122">Säilituspoliitika rakendamine postkastidele</span><span class="sxs-lookup"><span data-stu-id="a6c10-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="a6c10-123">Säilituse siltide lisamine või eemaldamine</span><span class="sxs-lookup"><span data-stu-id="a6c10-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="a6c10-124">Postkastile paigutatud ootelepaneku tüübi tuvastamine</span><span class="sxs-lookup"><span data-stu-id="a6c10-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
