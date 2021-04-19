---
title: Avalikele kaustadele juurdepääsu juhtimine Outlooki abil
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
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816736"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="1e3c5-102">Avalikele kaustadele juurdepääsu juhtimine Outlooki abil</span><span class="sxs-lookup"><span data-stu-id="1e3c5-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="1e3c5-103">Selleks et määrata, millistele kasutajatele outlooki abil avalikele kaustadele juurde pääsevad:</span><span class="sxs-lookup"><span data-stu-id="1e3c5-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="1e3c5-104">Kasuta `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="1e3c5-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="1e3c5-105">$true: Luba kasutajatel Outlookis avalikele kaustadele juurde pääseda</span><span class="sxs-lookup"><span data-stu-id="1e3c5-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="1e3c5-106">$false: Keela kasutaja juurdepääs Outlooki avalikele kaustadele.</span><span class="sxs-lookup"><span data-stu-id="1e3c5-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="1e3c5-107">See on vaikeväärtus.</span><span class="sxs-lookup"><span data-stu-id="1e3c5-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="1e3c5-108">Märkus. See protseduur saab juhtida ainult ühendusi Outlooki töölauarakenduses Windowsi klientrakendustega.</span><span class="sxs-lookup"><span data-stu-id="1e3c5-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="1e3c5-109">Kasutajad pääsevad avalikele kaustadele juurde OWA või Outlook for Maci kaudu.</span><span class="sxs-lookup"><span data-stu-id="1e3c5-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="1e3c5-110">Lisateavet leiate teemast [Outlookis avalike kaustadega](https://aka.ms/controlpf) seotud kontrollitud ühendused.</span><span class="sxs-lookup"><span data-stu-id="1e3c5-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
