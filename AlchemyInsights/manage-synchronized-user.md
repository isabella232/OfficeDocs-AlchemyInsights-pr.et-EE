---
title: Sünkroonitud kasutaja haldamine
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
- "9000609"
- "2444"
ms.openlocfilehash: 0dc2ecfa0bb5703c619dc1b2d6b4d517f999da0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823963"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Ei saa määrata põhimeiliaadressi, muuta kasutaja atribuute ega eemaldada/kustutada sünkroonitud kasutajat

Kui kataloogisünkroonimine on teie keskkonnas lubatud, ei saa microsoft 365 halduskeskuses mõnda kasutaja- või objektiatribuudi muuta.

Sünkroonitud kasutajate ja kõigi nende atribuutide täielikuks haldamiseks kasutage kohalikke active directory kasutajaid ja rühmade halduskonsooli (adsiedit.msc).  

Teise võimalusena saate sünkroonitud kasutajate üksikuid kasutajaid või atribuute powerShelli abil muuta, nagu on näidatud nendes levinud näidetes.

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
