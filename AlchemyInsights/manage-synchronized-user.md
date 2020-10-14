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
ms.openlocfilehash: 7bf7d3f00308ff6bc973cd52e09ca51c5fd0f45b
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451396"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Ei saa määrata esmast meiliaadressi, muuta kasutajate atribuute või eemaldada/kustutada sünkroonitud kasutajat

Kui teie keskkonna jaoks on lubatud kataloogi sünkroonimine, siis ei saa mõnda kasutaja või objekti atribuuti Microsoft 365 halduskeskus kasutades muuta.

Sünkroonitud kasutajate ja kõigi atribuutide täielikuks haldamiseks saate kasutada kohalikku Active Directory kasutajate ja rühmade halduskonsooli (ADSIEdit. msc).  

Teise võimalusena saate muuta üksikute kasutajate või atribuutide sünkroonitud kasutajatele PowerShelli abil, nagu on näidatud järgmistes levinud näidetes.

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
