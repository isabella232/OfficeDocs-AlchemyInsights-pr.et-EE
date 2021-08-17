---
title: Turbejoonte Microsoft Intune kasutamine Windows 10 seadmetes
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
ms.openlocfilehash: a94c6b72df3874ee80413adac86d60306175734b6ff28b2e015e05eec6f3838b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104340"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Turbejoonte Microsoft Intune kasutamine Windows 10 seadmetes

Intune'i turbealused aitavad kaitsta kasutajaid ja seadmeid. Turbealused on Windows sätete eel konfigureeritud rühmad, mida kasutatakse vastavate turberühmade soovitatud teadaolevate sätete ja vaikeväärtuste rühma rakendamiseks. Intune'i turbe alusprofiili loomisega loote malli, mis koosneb mitmest seadme konfiguratsiooniprofiilist.

Kui juurutate turbealused kasutajate või seadmete rühmadele, rakendatakse sätted seadmetele, mis käitavad Windows 10 uuemates versioonides. Näiteks lubab MDM-i turbealus (1) BitLockeri irdkettatele, (2) nõuab seadme vabastamiseks parooli ja (3) keelab elementaarse autentimise. Kui teie keskkonnas ei tööta vaikeväärtus, kohandage lähtejoont, et rakendada nõudeid, mida vajate.

Turbealused aitavad luua ka Microsoft 365. Järgmised eelised on järgmised.

- Turbealus sisaldab turbega seotud sätete parimaid tavasid ja soovitusi. Kuna Intune'i partnerid Windows turbemeeskonnaga, kes loob rühmapoliitikate jaoks alusjooned, põhinevad need soovitused tugevatel juhistel ja ulatuslikul kogemusel.
- Kui olete Intune'i uus kasutaja ja pole kindel, kust alustada, aitavad turbealused teil kiiresti luua ja juurutada turvalise profiili.
- Kui kasutate praegu rühmapoliitikat, on migreerimine Intune'i haldamise eesmärgil palju lihtsam turbejoonte abil, kuna need on intune'i sisse ehitatud ja sisaldavad haldamise tipptasemel võimalusi.

Lisateavet leiate teemast Windows [turbealused ja](https://go.microsoft.com/fwlink/?linkid=2141503) [Mobiilsideseadmete haldus.](https://go.microsoft.com/fwlink/?linkid=2141701)