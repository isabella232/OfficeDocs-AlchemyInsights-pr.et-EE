---
title: Ühiskaustu ei saa avada
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812543"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook ei saa avalike kaustadega ühendust luua

Kui avalike kaustade juurdepääs mõne kasutaja jaoks ei tööta, proovige teha järgmist.

Loo ühendus EKSO PowerShelliga ja konfigureerige probleemsel kasutajakontol parameeter DefaultPublicFolderMailbox, et see vastaks toimiva kasutajakonto parameetritele.

Nt

Get-postkast WorkingUser | FT DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Set-postkast ProblemUser-DefaultPublicFolderMailbox \<value from previous command>

Muudatuse jõustumiseks oodake vähemalt üks tund.

Kui probleem ei lahene, siis järgige [selle toimingu](https://aka.ms/pfcte) abil avalike kaustade Accessi probleemide tõrkeotsingut Outlooki abil.
 
**Outlooki kaudu avalike kaustade juurde pääsemiseks kasutatavate kasutajate kontrollimiseks**tehke järgmist.

1.  Kasuta Set-CASMailbox <mailboxname> -PublicFolderClientAccess $TRUE või $FALSE  
      
    $true: Outlookis avalike kaustade juurdepääsu lubamine kasutajatele  
      
    $false: Outlookis kasutajate juurdepääsu takistamine avalikesse kaustadesse See on vaikeväärtus.  
        
2.  Set-OrganizationConfig-PublicFolderShowClientControl $true   
      
**Märkus** Selle toiminguga saab ühendusi reguleerida ainult Outlooki töölaua Windowsi klientrakendustes. Kasutaja saab jätkata avalike kaustade juurdepääsu OWA või Outlook for Maci kaudu.
 
Lisateavet leiate teemast [Outlookis avalike kaustadesse toetatud ühenduste toe väljakuulutamine](https://aka.ms/controlpf).