---
title: Windows 10 seadmete konfigureerimine Microsoft Intune Security bases abil
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50694436"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>Microsoft Intune ' i turvalisuse alused Windows 10 seadmete konfigureerimiseks

Turvalisuse alused aitavad kaitsta kasutajaid ja seadmeid. Turvalisuse alused on Windowsi sätted ' eelkonfigureeritud rühmad, mida kasutatakse teadaolevate rühma sätete ja vastavate turbe-rühmade soovitatud vaikeväärtuste rakendamiseks. Kui loote Intune ' i turbe põhiprofiili, saate luua malli, mis koosneb mitmest seadme konfiguratsiooni profiilist.

Kui juurutate turvalisuse tasemeid kasutajate või seadmete rühmades, rakendatakse sätteid Windows 10 või uuemates versioonides töötavate seadmete suhtes. Näiteks Microsoft Mobile Device Management (MDM) Security Base automaatselt (1) lubab BitLocker for eemaldatavad draivid, (2) nõuab seadme lukustamise parooli ja (3) keelab põhiautentimise. Kui vaikeväärtus ei tööta teie keskkonna jaoks, saate kohandada algseid sätteid, et rakendada vajalikke sätteid.

Turvalisuse põhialused aitavad luua ka lõpuga turvalise töövoo Microsoft 365. Selle funktsiooni eelised on järgmised.
- Turvalisuse põhialus sisaldab turvalisust mõjutavatele sätetele häid tavasid ja soovitusi. Kuna Intune ' i partnerid Windowsi turvalisuse meeskonnaga, mis loob rühmapoliitika jaoks baseid, põhinevad need soovitused kindlatel juhistel ja laialdastel kogemustel.
- Kui teil on uus Intune ' is ja te pole kindel, kust alustada, siis turvalisuse alused aitavad teil kiiresti luua ja juurutada turvalist profiili.
- Kui kasutate praegu rühmapoliitika, siis migreerimine Intune ' i juhtimiseks on palju hõlpsam kui turvalisuse alused, sest need turvalisuse alused on loodud Intune ' i ja hõlmavad juhtimise tipptaseme võimalusi.

Lisateavet leiate teemast [Windowsi turvalisuse alused](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) ja [mobiilsideseadmete haldus](https://docs.microsoft.com/windows/client-management/mdm/).