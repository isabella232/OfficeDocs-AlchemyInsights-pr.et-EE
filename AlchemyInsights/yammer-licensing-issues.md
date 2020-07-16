---
title: Yammeri litsentsimise probleemid
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148236"
---
# <a name="yammer-licensing-issues"></a>Yammeri litsentsimise probleemid

Kõigil kasutajatel peab olema Yammer Enterprise'i teenuse kasutamiseks litsents, kuid vaikimisi ei nõua Yammer, et kasutajatel oleks teenusele juurdepääsuks litsents. Kui administraator muudab sätet, et blokeerida Microsoft 365 kasutajad ilma Yammeri litsentsideta, ei pääse Yammeri teenusele juurde kasutajad, kellele pole Yammerenterprise'i litsentsi määratud. Lisateavet leiate teemast [Yammeri kasutajalitsentside haldamine teenusekomplektis Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Kui litsentsid eemaldatakse kasutajatelt, ei kuvata enam Yammeri paani ja muud teenused saavad funktsioonide peitmiseks kasutada litsentsi eemaldamist. Muudel juhtudel võivad funktsioonid siiski ilmuda, kuid nõuavad litsentsi määramist.  

**Litsentsi ei värskendata kasutaja jaoks**  

Aeg-ajalt määratakse kasutajale litsents, kuid ei pääse endiselt Yammerile juurde. Viivitused on tõenäolisem, kui mass litsentsi määramine on pooleli. Yammeri kasutajaid ei pruugita värskendada samas järjekorras, kuna litsentse muudetakse Azure AD-s, kuna süsteem töötab asünkroonselt. Oodake kuni 24 tundi enne tugiteenuse juhtumi avamist, et teatada litsentsi sünkroonimisprobleemidest.  

**Hulgilitsentsi määramine**  

Litsentse saab määrata halduskeskuse või PowerShelli skriptimise kaudu. Lisateavet leiate teemast [Kasutajatele litsentside määramine](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ja [Kasutajakontodele litsentside määramine Office 365 PowerShelli abil.](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell) 

Microsofti tugiteenus ei paku abi skriptide loomisel, kuid Yammeri litsentsi määramise dokumentatsioon on saadaval. Lisateavet leiate teemast [Yammeri litsentside haldamine Windows PowerShelli abil](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).