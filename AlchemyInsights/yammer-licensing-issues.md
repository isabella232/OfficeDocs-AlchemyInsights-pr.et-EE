---
title: Yammeri litsentsimise probleemid
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
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657272"
---
# <a name="yammer-licensing-issues"></a>Yammeri litsentsimise probleemid

Kõigi kasutajate jaoks peab olema litsents Yammeri Enterprise ' i teenuse kasutamiseks, kuid vaikimisi ei nõua Yammeri kasutajatel teenusele juurdepääsuks litsentsi. Kui administraator muudab sätteid Microsoft 365 kasutajate blokeerimiseks ilma Yammeri litsentsideta, ei saa kasutajad, kellele on määratud Yammeri Enterprise ' i litsents, juurdepääsu Yammeri teenusele. Lisateavet leiate teemast [Yammeri kasutajate litsentside haldamine Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Kui litsentsid eemaldatakse kasutajatelt, ei kuvata enam Yammeri paani ja muud teenused saavad funktsioonide peitmiseks kasutada litsentside eemaldamist. Muudel juhtudel saab funktsioone endiselt näha, kuid vaja on kasutada litsentsi määramise funktsiooni.  

**Litsentsi ei saa kasutaja jaoks värskendada**  

Mõnikord määratakse kasutajale litsents, kuid Yammerile ei pääse endiselt juurde. Viivitusi esineb suurema tõenäosusega, kui on käimas massmälu määramine. Yammeri kasutajaid ei pruugita värskendada samas korralduses, nagu litsentsid on Azure AD-s muudetud, kuna süsteem töötab asünkroonselt. Oodake kuni 24 tundi, enne kui avate tugiteenuse juhtumi, et teatada litsentsi sünkroonimise probleemidest.  

**Litsentsi põhiosa määramine**  

Litsentse saab määrata administreerimiskeskuse või PowerShelli skriptimise kaudu. Lisateavet leiate teemast [kasutajatele litsentside määramine](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ja [Office 365 PowerShelli abil kasutajakontodele litsentside määramine](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Microsoft support ei paku skriptide loomisele abi, kuid saadaval on Yammeri litsentsi määramise dokumentatsioon. Lisateavet leiate teemast [Yammeri litsentside haldamine Windows PowerShelli abil](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).