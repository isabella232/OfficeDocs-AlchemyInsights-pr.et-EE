---
title: Avalikele kaustadele juurdepääsu Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 1386b97f804e63455094abf64b9d9e2541d57dafa36535813b0d7689e0ce2966
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032554"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Avalikele kaustadele juurdepääsu Outlook

Selleks et määrata, millistele kasutajatele pääsevad avalikud kaustad Outlook.

1. Kasuta `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: kasutajate juurdepääsu võimaldamine ühiskaustadele Outlook  
$false: Kasutaja juurdepääsu takistamine ühiskaustadele Outlook. See on vaikeväärtus.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Märkus. See protseduur saab juhtida ainult Outlook klientrakenduste Windows ühendusi. Kasutajad pääsevad edasi avalikele kaustadele juurde OWA või Outlook for Maci kaudu.

Lisateavet leiate teemast [Kontrollitud ühendused ühiskaustadega Outlook](https://aka.ms/controlpf) lisateavet.
