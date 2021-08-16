---
title: Muuda tugevat paroolinõuet
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
- "9000105"
- "1600"
ms.openlocfilehash: 8a82c002bd64a33556b632545e98355e860848d845e122bfea06fbc5ee5dcb90
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070680"
---
# <a name="change-strong-password-requirement"></a>Tugeva paroolinõude muutmine

Microsoft nõuab vaikimisi tugevaid paroole.

PowerShelli abil saate keelata kindlate kasutajate jaoks tugevad paroolid, kasutades järgmisi käske.

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Kõigi kasutajate jaoks tugevate paroolide keelamiseks kasutage:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Lisateave paroolipoliitika kohta](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [PowerShelli abil Microsoft 365 ühenduse loomine](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Lisateave PowerShelli MsolUseri käskude kohta](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
