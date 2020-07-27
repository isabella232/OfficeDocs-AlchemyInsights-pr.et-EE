---
title: Outlookis lisandmoodulite lisamise ajal on mitu kasutajat Accessi tõrgetega keelatud
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423717"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Outlookis lisandmoodulite lisamise ajal on mitu kasutajat Accessi tõrgetega keelatud

Saate määrata, millised teie asutuse administraatorid omavad Outlooki lisandmoodulite installimise ja haldamise õigust. Samuti saate määrata, millistel ettevõtte kasutajatel on õigus lisandmooduleid oma tarbeks installida ja hallata.

Lisateavet leiate teemast [administraatorite ja kasutajate määramine, kes saavad Outlooki lisandmooduleid installida ja hallata](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

Kui soovite kinnitada, et olete kasutaja jaoks kasutajale õiguse määranud, asendage selle <Role Name> rolli nimi, mida soovite kontrollida, ja käivitage järgmine käsk Exchange Online PowerShellis.

Get-ManagementRoleAssignment-roll " <Role Name> "-GetEffectiveUsers

Selles näites kirjeldatakse, kuidas kinnitada, kellele olete Office ' i poest Office ' i poest lisandmoodulite installimise õiguse määranud.

PowerShelli

-Roll "org turuplatsi rakendused"-GetEffectiveUsers

Tulemite ManagementRoleAssignment saate vaadata veerus tõhus kasutajad olevaid kandeid.

Üksikasjalikku teavet süntaksi ja parameetrite kohta leiate teemast [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 