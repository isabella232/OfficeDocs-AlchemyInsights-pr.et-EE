---
title: Office ' i juurutamise tööriista kasutamine
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085828"
---
# <a name="using-the-office-deployment-tool-odt"></a>Office ' i juurutamise tööriista (ODT) kasutamine

Office ' i juurutamise tööriista (ODT) abil saate Office ' i 365 Office ' i versioone juurutada. Office ' i juurutamise tööriist (setupodt.exe) käivitatakse käsurealt ja see kasutab konfiguratsiooni XML-faili, et määrata, milliseid sätteid Office ' i juurutamisel rakendada.
  
1. Laadige [Microsofti allalaadimiskeskusest](https://go.microsoft.com/fwlink/p/?LinkID=626065)alla Office ' i juurutamise tööriista uusim versioon.

2. Kasutage [Office ' i kohandamise tööriista (ÜMT)](https://config.office.com) juurutuse eelistuste valimiseks ja konfiguratsiooni XML-faili loomiseks. Eksportige konfiguratsioonifail ja paigutage see lokaalselt samasse kausta, kus asub setupodt.exe.

    **Märkus:** Office ' i installimisega seotud probleemid ilmnevad sageli valesti konfigureeritud või malformatted konfiguratsioonifailid. Selliste probleemide vältimiseks soovitame konfiguratsioonifaili loomiseks kasutada Office ' i kohandamise tööriista. Olemasolevaid konfiguratsiooniseadeid saate importida ka Office ' i kohandamise tööriista.

3. Liikuge tõstetud käsuviiba kaudu kohale, kus setupodt.exe asub, ja käivitage Office ' i juurutamise tööriist allalaaditavas režiimis ning määrake äsja salvestatud konfiguratsioonifail. Selles näites on konfiguratsioonifaili nimi Configuration.xml:

```setupodt.exe /download Configuration.xml```

4. Käivitage Office ' i juurutamise tööriist konfigureerimise režiimis ja määrake konfiguratsioonifail.

```setupodt.exe /configure Configuration.xml```

**Märkus:** Selle toimingu peate käivitama klientarvutis, kuhu soovite Office ' i installida, ja teil peavad olema kohaliku administraatori õigused selles arvutis.

Lisateavet Office ' i juurutamise tööriista kasutamise kohta Microsoft 365 rakenduste jaoks Enterprise ' i juurutamise stsenaariumide kohta leiate artiklist [Office ' i juurutamise tööriista ülevaade](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Lisateavet Office ' i kohandamise tööriista kasutamise kohta leiate teemast [Office ' i kohandamise tööriista ülevaade](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
