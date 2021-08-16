---
title: Yammer litsentsimisprobleemid
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 3ec764ece9cb7be933e9e2cd002379898522790528b0fa586ab501424b00cd7b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989725"
---
# <a name="yammer-licensing-issues"></a>Yammer litsentsimisprobleemid

Kõigil kasutajatel peab olema teenuse kasutamiseks Yammer Enterprise litsents, kuid vaikimisi ei Yammer kasutajatele teenusele juurdepääsuks litsentsi. Kui administraator muudab sätet, et blokeerida Microsoft 365 ilma Yammer litsentsideta, ei pääse kasutajad, kellele pole Yammer Enterprise litsentsi, juurdepääsu Yammer teenusele. Lisateavet leiate teemast [Kasutajalitsentside Yammer haldamine Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Kui litsentsid eemaldatakse kasutajatelt, ei Yammer enam paani ja muud teenused saavad funktsioonide peitmiseks kasutada litsentsi eemaldamist. Muudel juhtudel võivad funktsioonid siiski ilmuda, kuid nende toimimiseks on vaja litsentsi määramist.  

**Kasutaja litsentsi ei värskendata**  

Aeg-ajalt määratakse kasutajale litsents, kuid ta ei pääse Yammer. Viivitused ilmnevad suurema tõenäosusega siis, kui hulgilitsentsi määramine on pooleli. Yammer ei pruugita azure AD-s litsentsidega samas järjestuses värskendada, kuna süsteem töötab asünkroonselt. Litsentsisünkroonimisprobleemidest teatamine võib oodata kuni 24 tundi enne tugiteenuse juhtumi avamist.  

**Hulgilitsentsi määramine**  

Litsentse saab määrata halduskeskuse või PowerShelli skriptimise kaudu. Lisateavet leiate teemast [Litsentside määramine](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) kasutajatele ja Litsentside määramine kasutajakontodele [PowerShelli Office 365 abil.](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell) 

Microsofti tugiteenused ei paku abi skriptide loomisel, kuid dokumentatsiooni Yammer litsentsi määramine on saadaval. Lisateavet leiate teemast Yammer [litsentside haldamine Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).