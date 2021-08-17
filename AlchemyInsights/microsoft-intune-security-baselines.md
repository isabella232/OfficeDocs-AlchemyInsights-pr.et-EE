---
title: Turbejoonte Microsoft Intune kasutamine Windows 10 seadmetes
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: f77fdbb315db8317a6a1374f05489a7f5a0bedcec484dc9ac53a473098583949
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57886628"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Turbejoonte Microsoft Intune kasutamine Windows 10 seadmetes

Intune'i turbealused aitavad kaitsta kasutajaid ja seadmeid. Turbealused on Windows eel konfigureeritud rühmad, mida kasutatakse vastavate turberühmade soovitatud teadaolevate sätete ja vaikeväärtuste rühma rakendamiseks. Intune'i turbe alusprofiili loomisega loote malli, mis koosneb mitmest seadme konfiguratsiooniprofiilist.

Kui juurutate turbealused kasutajate või seadmete rühmadele, rakendatakse sätted seadmetele, mis Windows 10 või uuemates versioonides. Näiteks lubab Microsofti mobiilsideseadmete halduse (MDM) turbealus BitLockeri irdkettatele automaatselt, nõuab seadme vabastamiseks parooli ja keelab elementaarse autentimise. Kui teie keskkonnas vaikeväärtus ei tööta, saate kohandada lähtejoont, et rakendada nõudeid, mida vajate.

Turbealused aitavad luua ka Microsoft 365. Turbealus sisaldab turbega seotud sätete parimaid tavasid ja soovitusi. Intune'i partnerid Windows, mis loob rühmapoliitikate jaoks lähtealused, seega põhinevad need soovitused tugevatel juhistel ja ulatuslikul kogemusel.

Kui te pole Intune'i kasutusele võtnud ja pole kindel, kust alustada, aitavad turbealused kiiresti luua ja juurutada turvalise profiili. Kui kasutate praegu rühmapoliitikat, on migreerimine Intune'i haldamise eesmärgil palju lihtsam turbealustega, kuna need on intune'i sisse ehitatud ja sisaldavad tipptasemel haldusfunktsioone.

Lisateavet leiate teemast Windows [turbealused ja](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) [Mobiilsideseadmete haldus.](https://docs.microsoft.com/windows/client-management/mdm/)

