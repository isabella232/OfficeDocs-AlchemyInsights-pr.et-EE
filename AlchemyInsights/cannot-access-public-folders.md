---
title: Ühiskaustu ei saa avada
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: d63a193585cb73c2ce8e160d413db4e837100d33
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341399"
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