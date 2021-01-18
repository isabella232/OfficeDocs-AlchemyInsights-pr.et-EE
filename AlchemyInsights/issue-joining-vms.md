---
title: Probleem ühendava VMs-ga
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885207"
---
# <a name="issue-joining-vms"></a>Probleem ühendava VMs-ga

VMs-ga liitumisel ilmnevate probleemide lahendamiseks tehke järgmist.

1. Proovige logida sisse **UPN** -vormingus (nt "joeuser@contoso.com") **sAMAccountName** vormingu asemel ("CONTOSO\joeuser").
2. Veenduge, et olete lubanud parooli sünkroonimise vastavalt juhistele, mida on kirjeldatud *jaotises Alustamine.*
3. Veenduge, et mõjutatud kasutajakonto poleks Azure AD rentniku väline konto. Välised kasutajad ei saa hallatavasse domeeni sisse logida, sest Azure AD Domain Services ei ole mandaati selliste kasutajakontode jaoks.
4. Kui mõjutatud kasutajakonto on pilveteenuse kasutaja konto, veenduge, et kasutajad on pärast Azure AD Domain Services lubanud parooli muutnud. See toiming põhjustab Azure AD Domain Services genereerimiseks nõutavate mandaatide hashes.
5. Kui mõjutatud Kasutajakontod sünkroonitakse kohapealsest kataloogist, veenduge, et Azure AD Connecti soovitatav versioon oleks konfigureeritud täieliku sünkroonimise sooritamiseks.
6. Kui probleemid püsivad pärast juhise 4 kinnitamist, käivitage sünkroonimisel arvuti kaudu järgmised käsud.
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.