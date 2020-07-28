---
title: Kasutajanime ei saa muuta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439099"
---
# <a name="unable-to-change-username"></a>Kasutajanime ei saa muuta

Mõnel juhul ei levitata UPN-i (UserPrincipalName) muutusi pilve. Võidakse kuvada Office 365 portaalis valideerimise tõrked või muuta kasutajanime või meiliaadressi. Probleemi lahendamiseks seadke UserPrincipalName käsitsi selle PowerShelli käsu abil.

**Näide: kasutaja ümbernimetamine**

PowerShellCopy

PS C: \> Set-MsolUserPrincipalName-userPrincipalName "davidc@contoso.com"-NewUserPrincipalName "davidchew@contoso.com"

Selle käsuga nimetatakse davidc@contoso.com davidchew@contoso.com.

Lisateavet leiate teemast [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).