---
title: Sünkroonitud kasutaja haldamine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 84e337a7224fdd3c3ab7ad0f61240692fe007d5a
ms.sourcegitcommit: 82af227ac6d075e748e27c4ce6bdcf56628559cb
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/28/2020
ms.locfileid: "44407346"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="bf5e5-102">Ei saa seada esmane meiliaadress, muuta kasutaja atribuute või eemaldada/kustutada sünkroonitud kasutaja</span><span class="sxs-lookup"><span data-stu-id="bf5e5-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="bf5e5-103">Kui kataloogi sünkroonimine on lubatud teie keskkonnas, mõned kasutaja või objekti atribuute ei saa muuta, kasutades Microsoft 365 halduskeskus.</span><span class="sxs-lookup"><span data-stu-id="bf5e5-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="bf5e5-104">Sünkroonitud kasutajate ja kõigi nende atribuutide täielikuks haldamiseks kasutage kohalikku Active Directory kasutajate ja rühmade halduskonsooli (ADSIEdit. msc).</span><span class="sxs-lookup"><span data-stu-id="bf5e5-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="bf5e5-105">Teise võimalusena saate muuta üksikuid kasutajaid või atribuute sünkroonitud kasutajatele PowerShelli abil, nagu on näidatud nende levinud näidetes:</span><span class="sxs-lookup"><span data-stu-id="bf5e5-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
