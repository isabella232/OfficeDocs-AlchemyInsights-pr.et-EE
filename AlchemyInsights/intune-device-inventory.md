---
title: Intune'i seadme inventuur
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 00ee4f1d7130c239272e28ee8e051a18e6e0baf13040d2a892866be5900adfaf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54014068"
---
# <a name="intune-device-inventory"></a>Intune'i seadme inventuur

Seadmesaba annab administraatorile ülevaate Intune'i halduses olevast seadmest seadme kohta. Kuvatava teabe hulka kuuluvad riistvara, leitud rakendused, seadme nõuetele vastavuse olek ja seadme konfiguratsiooni olek.

Riistvara ja avastatud rakenduste laoandmeid kogutakse seitsme päeva jooksul. Teatatud riistvararakendused ja konkreetsed elemendid erinevad olenevalt seadme opsüsteemist ja sellest, kas seade kuulub isiklikult või ettevõttele.

Lisateavet leiate teemast [Intune'i seadme üksikasjade kuvamine.](https://docs.microsoft.com/intune/device-inventory)

**KKK**

Küsimus. Ma ei saa intune'i registreeritud seadmetes Windows. Miks mitte?

A. Praegu loetletakse ettevõtte seadmetena Windows 10 arvutite jaoks ainult tänapäevased rakendused. Intune ei kogu teavet nendesse seadmetesse installitud Win32 rakenduste kohta.

Küsimus. Miks ei koguta telefoninumbreid kõigilt seadmetelt?

A. Intune'is ettevõtte seadmeteks liigitatud telefone ei tuvastata täistelefoninumbriga, kui käivitate näiteks mobiilsideseadme varude aruande. Oma seadme telefoninumbrite toomine on alati osaliselt maskeeritud tärnidega (****) ja kuvatakse ainult neli viimast numbrit.