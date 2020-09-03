---
title: Ühiskaustu ei saa avada
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: d63a193585cb73c2ce8e160d413db4e837100d33
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341399"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="3f8a3-102">Outlook ei saa avalike kaustadega ühendust luua</span><span class="sxs-lookup"><span data-stu-id="3f8a3-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="3f8a3-103">Kui avalike kaustade juurdepääs mõne kasutaja jaoks ei tööta, proovige teha järgmist.</span><span class="sxs-lookup"><span data-stu-id="3f8a3-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="3f8a3-104">Loo ühendus EKSO PowerShelliga ja konfigureerige probleemsel kasutajakontol parameeter DefaultPublicFolderMailbox, et see vastaks toimiva kasutajakonto parameetritele.</span><span class="sxs-lookup"><span data-stu-id="3f8a3-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="3f8a3-105">Nt</span><span class="sxs-lookup"><span data-stu-id="3f8a3-105">Example:</span></span>

<span data-ttu-id="3f8a3-106">Get-postkast WorkingUser | FT DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="3f8a3-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="3f8a3-107">Set-postkast ProblemUser-DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="3f8a3-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="3f8a3-108">Muudatuse jõustumiseks oodake vähemalt üks tund.</span><span class="sxs-lookup"><span data-stu-id="3f8a3-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="3f8a3-109">Kui probleem ei lahene, siis järgige [selle toimingu](https://aka.ms/pfcte) abil avalike kaustade Accessi probleemide tõrkeotsingut Outlooki abil.</span><span class="sxs-lookup"><span data-stu-id="3f8a3-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="3f8a3-110">**Outlooki kaudu avalike kaustade juurde pääsemiseks kasutatavate kasutajate kontrollimiseks**tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="3f8a3-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="3f8a3-111">Kasuta Set-CASMailbox <mailboxname> -PublicFolderClientAccess $TRUE või $FALSE</span><span class="sxs-lookup"><span data-stu-id="3f8a3-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="3f8a3-112">$true: Outlookis avalike kaustade juurdepääsu lubamine kasutajatele</span><span class="sxs-lookup"><span data-stu-id="3f8a3-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="3f8a3-113">$false: Outlookis kasutajate juurdepääsu takistamine avalikesse kaustadesse</span><span class="sxs-lookup"><span data-stu-id="3f8a3-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="3f8a3-114">See on vaikeväärtus.</span><span class="sxs-lookup"><span data-stu-id="3f8a3-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="3f8a3-115">Set-OrganizationConfig-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="3f8a3-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="3f8a3-116">**Märkus** Selle toiminguga saab ühendusi reguleerida ainult Outlooki töölaua Windowsi klientrakendustes.</span><span class="sxs-lookup"><span data-stu-id="3f8a3-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="3f8a3-117">Kasutaja saab jätkata avalike kaustade juurdepääsu OWA või Outlook for Maci kaudu.</span><span class="sxs-lookup"><span data-stu-id="3f8a3-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="3f8a3-118">Lisateavet leiate teemast [Outlookis avalike kaustadesse toetatud ühenduste toe väljakuulutamine](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="3f8a3-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>