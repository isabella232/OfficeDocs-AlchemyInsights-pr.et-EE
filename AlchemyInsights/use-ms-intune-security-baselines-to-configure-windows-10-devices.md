---
title: Windows 10 seadmete konfigureerimine Microsoft Intune Security bases abil
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573401"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Windows 10 seadmete konfigureerimine Microsoft Intune Security bases abil

Turvalisuse alused aitavad kaitsta kasutajaid ja seadmeid. Turvalisuse alused on Windowsi sätted ' eelkonfigureeritud rühmad, mida kasutatakse teadaolevate rühma sätete ja vastavate turbe-rühmade soovitatud vaikeväärtuste rakendamiseks. Kui loote Intune ' i turbe põhiprofiili, saate luua malli, mis koosneb mitmest seadme konfiguratsiooni profiilist.

Kui juurutate turvalisuse tasemeid kasutajate või seadmete rühmades, rakendatakse sätteid Windows 10 või uuema versiooniga töötavate seadmete jaoks. Näiteks MDM Security Base automaatselt (1) lubab BitLocker for eemaldatavad draivid, (2) nõuab seadme lukustamise parooli ja (3) keelab põhiautentimise. Kui vaikeväärtus ei tööta teie keskkonna jaoks, kohandage võrdlusalust, et rakendada vajalikke sätteid.

Turvalisuse põhialused aitavad luua ka lõpuga turvalise töövoo Microsoft 365. Järgmised eelised on järgmised.

- Turvalisuse põhialus sisaldab turvalisust mõjutavatele sätetele häid tavasid ja soovitusi. Kuna Intune ' i partnerid Windowsi turvalisuse meeskonnaga, mis loob rühmapoliitika jaoks baseid, põhinevad need soovitused kindlatel juhistel ja laialdastel kogemustel.
- Kui teil on uus Intune ' is ja te pole kindel, kust alustada, siis turvalisuse alused aitavad teil kiiresti luua ja juurutada turvalist profiili.
- Kui kasutate praegu rühmapoliitika, siis migreerimine Intune ' i juhtimiseks on palju hõlpsam, sest need on loodud Intune ' i ja hõlmavad ka juhtimise tipptaseme võimalusi.

Lisateavet leiate teemast [Windowsi turvalisuse alused](https://go.microsoft.com/fwlink/?linkid=2141503) ja [mobiilsideseadmete haldus](https://go.microsoft.com/fwlink/?linkid=2141701).