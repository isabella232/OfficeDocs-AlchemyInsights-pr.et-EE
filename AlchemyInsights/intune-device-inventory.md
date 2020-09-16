---
title: Seadme laoseisu häälestamine
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
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667874"
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