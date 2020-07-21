---
title: Orvuks kasutaja kustutamine asutusesisesest serverist
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/20/2020
ms.locfileid: "45197940"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="cb308-102">Orvuks kasutaja kustutamine asutusesisesest serverist</span><span class="sxs-lookup"><span data-stu-id="cb308-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="cb308-103">Orvuks kasutaja eemaldamiseks toimige järgmiselt.</span><span class="sxs-lookup"><span data-stu-id="cb308-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="cb308-104">Sundida kataloogi sünkroonimine, järgides juhiseid [Mis on hübriid identiteedi Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="cb308-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="cb308-105">Kataloogi sünkroonimise kontrollimiseks vaadake teemat [Mis on hübriididentiteet Azure Active Directoryga?](https://technet.microsoft.com/library/jj151797.aspx)</span><span class="sxs-lookup"><span data-stu-id="cb308-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="cb308-106">Kui sünkroonimine toimib õigesti, kuid Active Directory objekti kustutamine ei levi Azure AD, käsitsi eemaldada orvuks objekti, kasutades ühte järgmistest Azure Active Directory moodul Windows PowerShelli cmdlet-käsud:</span><span class="sxs-lookup"><span data-stu-id="cb308-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="cb308-107">Eemalda MsolContact</span><span class="sxs-lookup"><span data-stu-id="cb308-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="cb308-108">Eemalda MsolGroup</span><span class="sxs-lookup"><span data-stu-id="cb308-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="cb308-109">Eemalda MsolUser</span><span class="sxs-lookup"><span data-stu-id="cb308-109">Remove-MsolUser</span></span>

    <span data-ttu-id="cb308-110">Näiteks orvuks kasutaja ID john.smith@contoso.com eemaldamiseks, mis loodi algselt kataloogi sünkroonimise abil, käivitage cmdlet-käsk:</span><span class="sxs-lookup"><span data-stu-id="cb308-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="cb308-111">Eemalda MsolUser –UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="cb308-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>