---
title: Sünkroonitud kasutaja haldamine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 53c188f6c6ab93bcc6f87d95717dc0d24d492bb7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47777673"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="492e0-102">Ei saa määrata esmast meiliaadressi, muuta kasutajate atribuute või eemaldada/kustutada sünkroonitud kasutajat</span><span class="sxs-lookup"><span data-stu-id="492e0-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="492e0-103">Kui teie keskkonna jaoks on lubatud kataloogi sünkroonimine, siis ei saa mõnda kasutaja või objekti atribuuti Microsoft 365 halduskeskus kasutades muuta.</span><span class="sxs-lookup"><span data-stu-id="492e0-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="492e0-104">Sünkroonitud kasutajate ja kõigi atribuutide täielikuks haldamiseks saate kasutada kohalikku Active Directory kasutajate ja rühmade halduskonsooli (ADSIEdit. msc).</span><span class="sxs-lookup"><span data-stu-id="492e0-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="492e0-105">Teise võimalusena saate muuta üksikute kasutajate või atribuutide sünkroonitud kasutajatele PowerShelli abil, nagu on näidatud järgmistes levinud näidetes.</span><span class="sxs-lookup"><span data-stu-id="492e0-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
