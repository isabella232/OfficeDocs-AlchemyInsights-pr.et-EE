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
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380501"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="6fec6-102">Esmane e-posti aadressi või kasutaja atribuute muuta ei saa</span><span class="sxs-lookup"><span data-stu-id="6fec6-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="6fec6-103">Kui kataloogi sünkroonimine on lubatud teie keskkonnas mõned kasutaja või objekti atribuute ei saa muuta halduskeskuse.</span><span class="sxs-lookup"><span data-stu-id="6fec6-103">If directory synchronization is enabled for your environment some user or object attributes cannot be changed using the Admin Center.</span></span>
<span data-ttu-id="6fec6-104">Täielikult sünkroniseeritud kasutajate ja nende atribuutide haldamiseks kasutage oma kohaliku active directory kasutajate ja rühmade halduskonsooli (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="6fec6-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="6fec6-105">Teise võimalusena saate muuta kasutajatele või atribuutide sünkroonitud kasutajad nagu näidatud ühise nendes näidetes PowerShelli:</span><span class="sxs-lookup"><span data-stu-id="6fec6-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="6fec6-106">Set-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="6fec6-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="6fec6-107">Set-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Testkasutaja" - perekonnanimi "Kasutaja"-pealkiri "Manager"-osakond "HR"</span><span class="sxs-lookup"><span data-stu-id="6fec6-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="6fec6-108">Eemalda MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="6fec6-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>