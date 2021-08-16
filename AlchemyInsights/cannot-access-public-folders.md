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
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996626"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook ei saa avalike kaustadega ühendust luua

Kui ühiskausta juurdepääs ei tööta mõne kasutaja jaoks, proovige järgmist.

Ühendus exo PowerShelli ja konfigureerige probleemse kasutajakonto parameeter DefaultPublicFolderMailbox nii, et see vastaks töökonto parameetrile.

Näide:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Muudatuse jõustumist oodake vähemalt üks tund.

Kui probleem ei kordu, järgige avaliku [kausta](https://aka.ms/pfcte) juurdepääsu probleemide tõrkeotsinguks seda Outlook.
 
**Selleks et määrata, millistele kasutajatele on juurdepääs avalikele kaustadele Outlook.**

1.  Kasutage Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true või $false  
      
    $true: kasutajate juurdepääsu võimaldamine ühiskaustadele Outlook  
      
    $false: Kasutaja juurdepääsu takistamine ühiskaustadele Outlook. See on vaikeväärtus.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Märkus** See protseduur saab juhtida ühendusi ainult Outlook töölauarakenduste Windows kaudu. Kasutaja saab jätkata avalikele kaustadele juurdepääsu OWA või Outlook for Maci abil.
 
Lisateavet leiate teemast [Ühiskaustade](https://aka.ms/controlpf)kontrollitud ühenduste toe Outlook.