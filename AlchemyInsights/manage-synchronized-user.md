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
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Esmane e-posti aadressi või kasutaja atribuute muuta ei saa

Kui kataloogi sünkroonimine on lubatud teie keskkonnas mõned kasutaja või objekti atribuute ei saa muuta halduskeskuse.
Täielikult sünkroniseeritud kasutajate ja nende atribuutide haldamiseks kasutage oma kohaliku active directory kasutajate ja rühmade halduskonsooli (adsiedit.msc).  

Teise võimalusena saate muuta kasutajatele või atribuutide sünkroonitud kasutajad nagu näidatud ühise nendes näidetes PowerShelli: 
- Set-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Set-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Testkasutaja" - perekonnanimi "Kasutaja"-pealkiri "Manager"-osakond "HR"
- Eemalda MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com