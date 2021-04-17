---
title: Avalikele kaustadele ei pääse juurde
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
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819508"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook ei saa avalike kaustadega ühendust luua

Kui ühiskausta juurdepääs ei tööta mõne kasutaja jaoks, proovige järgmist.

Looge ühendus EXO PowerShelliga ja konfigureerige probleemse kasutajakonto parameeter DefaultPublicFolderMailbox nii, et see vastaks töökonto parameetrile.

Näide:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Muudatuse jõustumist oodake vähemalt üks tund.

Kui probleem ei kordu, järgige [seda protseduuri](https://aka.ms/pfcte) avaliku kausta juurdepääsu probleemide tõrkeotsinguks Outlooki abil.
 
**Selleks, et määrata, millistele kasutajatele pääsevad Outlooki abil juurde ühiskaustadele:**

1.  Kasutage Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true või $false  
      
    $true: Luba kasutajatel Outlookis avalikele kaustadele juurde pääseda  
      
    $false: Keela kasutaja juurdepääs Outlooki avalikele kaustadele. See on vaikeväärtus.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Märkus** See protseduur saab kontrollida ühendusi ainult Outlooki töölauarakenduses Windowsi klientrakendustes. Kasutaja saab avalikele kaustadele juurde pääseda ka OWA või Outlook for Maci abil.
 
Lisateavet leiate teemast Outlookis avalike kaustadega seotud kontrollitud [ühenduste tugiteenustest teatamine.](https://aka.ms/controlpf)