---
title: Avalikele kaustadele juurdepääsu juhtimine Outlooki abil
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
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816736"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Avalikele kaustadele juurdepääsu juhtimine Outlooki abil

Selleks et määrata, millistele kasutajatele outlooki abil avalikele kaustadele juurde pääsevad:

1. Kasuta `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Luba kasutajatel Outlookis avalikele kaustadele juurde pääseda  
$false: Keela kasutaja juurdepääs Outlooki avalikele kaustadele. See on vaikeväärtus.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Märkus. See protseduur saab juhtida ainult ühendusi Outlooki töölauarakenduses Windowsi klientrakendustega. Kasutajad pääsevad avalikele kaustadele juurde OWA või Outlook for Maci kaudu.

Lisateavet leiate teemast [Outlookis avalike kaustadega](https://aka.ms/controlpf) seotud kontrollitud ühendused.
