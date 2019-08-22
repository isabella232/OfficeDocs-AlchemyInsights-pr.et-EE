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
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36541983"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Esmane e-posti aadressi või kasutaja atribuute muuta ei saa

Kui kataloogi sünkroonimine on lubatud teie keskkonnas, mõned kasutaja või objekti atribuute ei saa muuta Microsoft 365 halduskeskuse.

Täielikult sünkroniseeritud kasutajate ja nende atribuutide haldamiseks kasutage oma kohaliku active directory kasutajate ja rühmade halduskonsooli (adsiedit.msc).  

Teise võimalusena saate muuta kasutajatele või atribuutide sünkroonitud kasutajad nagu näidatud ühise nendes näidetes PowerShelli: 
- Set-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Set-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Testkasutaja" - perekonnanimi "Kasutaja"-pealkiri "Manager"-osakond "HR"
- Eemalda MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com