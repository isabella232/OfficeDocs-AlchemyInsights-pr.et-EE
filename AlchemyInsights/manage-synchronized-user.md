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
ms.openlocfilehash: bfa66492397adfd121fd3c9ddb2c190394cbc9a771a3e2c2db656ad438e404f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114772"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Ei saa määrata põhimeiliaadressi, muuta kasutaja atribuute ega eemaldada/kustutada sünkroonitud kasutajat

Kui kataloogisünkroonimine on teie keskkonnas lubatud, ei saa mõnda kasutaja- või objektiatribuudi Microsoft 365 halduskeskus.

Sünkroonitud kasutajate ja kõigi nende atribuutide täielikuks haldamiseks kasutage kohalikke active directory kasutajaid ja rühmade halduskonsooli (adsiedit.msc).  

Teise võimalusena saate sünkroonitud kasutajate üksikuid kasutajaid või atribuute powerShelli abil muuta, nagu on näidatud nendes levinud näidetes.

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
