---
title: Mitu kasutajat, kes ei näe Outlookis lisandmooduleid
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197841"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Mitu kasutajat, kes ei näe Outlookis lisandmooduleid

Kui testite Outlooki lisandmoodulid ja ükski kuvatakse, esimese tõrkeotsingu samm, kasutage **cmdlet-käsu Get-OrganizationConfig** PowerShelli päringu _AppsForOfficeEnabled_ parameeter. Kui päring tagastab väärtuse **False**, seadke selle parameetri **väärtuseks True** **set-OrganizationConfig cmdlet-käsu** abil, nii et lisandmoodulid kuvatakse ootuspäraselt.

Me ei soovita, et _AppsForOfficeEnabled_ parameeter on seatud **false**. **Väär** väärtus alistab kõik ülaltoodud haldus- ja kasutajarollisätted ja takistab organisatsiooni mis tahes kasutaja aktiveerimist uute rakenduste poolt.

Lisateabe saamiseks vaadake teemat [Outlooki lisandmoodulite installimiseks ja haldamiseks administraatorite ja kasutajate määramine](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).