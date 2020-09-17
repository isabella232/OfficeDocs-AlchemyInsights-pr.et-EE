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
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Ei saa määrata esmast meiliaadressi, muuta kasutajate atribuute või eemaldada/kustutada sünkroonitud kasutajat

Kui teie keskkonna jaoks on lubatud kataloogi sünkroonimine, siis ei saa mõnda kasutaja või objekti atribuuti Microsoft 365 halduskeskus kasutades muuta.

Sünkroonitud kasutajate ja kõigi atribuutide täielikuks haldamiseks saate kasutada kohalikku Active Directory kasutajate ja rühmade halduskonsooli (ADSIEdit. msc).  

Teise võimalusena saate muuta üksikute kasutajate või atribuutide sünkroonitud kasutajatele PowerShelli abil, nagu on näidatud järgmistes levinud näidetes. 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
