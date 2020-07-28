---
title: Seadme laoseisu häälestamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439160"
---
# <a name="intune-device-inventory"></a>Seadme laoseisu häälestamine

Seadmete Blade annab haldurile ülevaate halduses olevatest seadmetest, mida saab seadme põhjal häälestada. Kuvatud teave sisaldab: riistvara, avastatud rakendusi, seadme nõuetele vastavuse olekut ja seadme konfigureerimise olekut.

Riistvara ja avastatud rakenduste laoseisu andmed kogutakse seitsme päeva jooksul. Teatatud riistvara rakendused ja konkreetsed elemendid erinevad olenevalt seadme opsüsteemist ja sellest, kas seade on ise või ettevõtte omanduses.

Lisateavet leiate teemast [seadme üksikasjade kuvamine Intune ' is](https://docs.microsoft.com/intune/device-inventory).

**KKK**

K: ma ei saa täieliku laoseisu taotluste loendit Windowsi seadmetes. Miks mitte?

V: praegu on ainult moodsad rakendused loetletud Windows 10 arvutites, mis on tähistatud ettevõtte seadmetena. Intune ei kogu teavet nendesse seadmetesse installitud Win32 rakenduste kohta.

K: Miks ei koguta telefoninumbreid kõigilt seadmetelt?

V: telefonid, mis on kategoriseeritud kui ettevõtte seadmed Intune ' is, ei ole määratud nende täieliku telefoninumbriga, kui käivitate näiteks mobiilsideseadme laovarude aruandeid. Bring-you-oma-seadme telefoninumbrid on alati osaliselt maskid tärnide (* * * *) ja näidata ainult neli viimast numbrit.