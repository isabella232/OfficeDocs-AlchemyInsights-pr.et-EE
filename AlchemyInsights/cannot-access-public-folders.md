---
title: Avalikele kaustadele ei pääse juurde
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819508"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="cdeb2-102">Outlook ei saa avalike kaustadega ühendust luua</span><span class="sxs-lookup"><span data-stu-id="cdeb2-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="cdeb2-103">Kui ühiskausta juurdepääs ei tööta mõne kasutaja jaoks, proovige järgmist.</span><span class="sxs-lookup"><span data-stu-id="cdeb2-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="cdeb2-104">Looge ühendus EXO PowerShelliga ja konfigureerige probleemse kasutajakonto parameeter DefaultPublicFolderMailbox nii, et see vastaks töökonto parameetrile.</span><span class="sxs-lookup"><span data-stu-id="cdeb2-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="cdeb2-105">Näide:</span><span class="sxs-lookup"><span data-stu-id="cdeb2-105">Example:</span></span>

<span data-ttu-id="cdeb2-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="cdeb2-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="cdeb2-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="cdeb2-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="cdeb2-108">Muudatuse jõustumist oodake vähemalt üks tund.</span><span class="sxs-lookup"><span data-stu-id="cdeb2-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="cdeb2-109">Kui probleem ei kordu, järgige [seda protseduuri](https://aka.ms/pfcte) avaliku kausta juurdepääsu probleemide tõrkeotsinguks Outlooki abil.</span><span class="sxs-lookup"><span data-stu-id="cdeb2-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="cdeb2-110">**Selleks, et määrata, millistele kasutajatele pääsevad Outlooki abil juurde ühiskaustadele:**</span><span class="sxs-lookup"><span data-stu-id="cdeb2-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="cdeb2-111">Kasutage Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true või $false</span><span class="sxs-lookup"><span data-stu-id="cdeb2-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="cdeb2-112">$true: Luba kasutajatel Outlookis avalikele kaustadele juurde pääseda</span><span class="sxs-lookup"><span data-stu-id="cdeb2-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="cdeb2-113">$false: Keela kasutaja juurdepääs Outlooki avalikele kaustadele.</span><span class="sxs-lookup"><span data-stu-id="cdeb2-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="cdeb2-114">See on vaikeväärtus.</span><span class="sxs-lookup"><span data-stu-id="cdeb2-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="cdeb2-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="cdeb2-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="cdeb2-116">**Märkus** See protseduur saab kontrollida ühendusi ainult Outlooki töölauarakenduses Windowsi klientrakendustes.</span><span class="sxs-lookup"><span data-stu-id="cdeb2-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="cdeb2-117">Kasutaja saab avalikele kaustadele juurde pääseda ka OWA või Outlook for Maci abil.</span><span class="sxs-lookup"><span data-stu-id="cdeb2-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="cdeb2-118">Lisateavet leiate teemast Outlookis avalike kaustadega seotud kontrollitud [ühenduste tugiteenustest teatamine.](https://aka.ms/controlpf)</span><span class="sxs-lookup"><span data-stu-id="cdeb2-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>