---
title: Office juurutamise tööriista kasutamine
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
ms.openlocfilehash: 39a011d4b121492d222ff620e70d9860231b7bcfe0d7fd2ecfd93de1ef502f5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083766"
---
# <a name="using-the-office-deployment-tool-odt"></a>Tööriista Office (ODT) kasutamine

Office juurutamise tööriista (ODT) Office 365 versiooni Office. Office juurutustööriista (setup.exe) käivitatakse käsurealt ja see määratleb konfiguratsiooni XML-faili abil, milliseid sätteid Office.
  
1. Laadige Microsofti allalaadimiskeskusest alla Office juurutamise tööriista [uusim versioon.](https://go.microsoft.com/fwlink/p/?LinkID=626065)

2. [Juurutuseeelistuste](https://config.office.com) valimiseks ja konfiguratsiooni XML-faili loomiseks saate kasutada Office -i kohandamistööriista (OCT). Eksportige konfiguratsioonifail ja paigutage see kohalikult samasse kausta, kus setup.exe asub.

    **Märkus.** Office installiprobleemid ilmnevad sageli valesti konfigureeritud või valesti vormindatud konfiguratsioonifailide tõttu. Selliste probleemide vältimiseks soovitame kasutada konfiguratsioonifaili Office kohandamise tööriista. Samuti saate olemasolevaid konfiguratsioonifaile importida Office kohandamistööriista.

3. Aktiveerige administraatoriõigustega käsuviiba kaudu koht, kus setup.exe asub, ja käivitage Office juurutamise tööriist allalaadimisrežiimis ja määrake äsja salvestatud konfiguratsioonifail. Selles näites on konfiguratsioonifaili nimi Configuration.xml.

```setup.exe /download Configuration.xml```

4.Käivitage Office juurutamise tööriist konfigureerimisrežiimis ja määrake konfiguratsioonifail.

```setup.exe /configure Configuration.xml```

**Märkus.** Selle juhise peate käivitama klientarvutist, kuhu soovite Office, ja teil peavad olema selles arvutis kohaliku administraatori õigused.

Lisateavet juurutamistööriista Office juurutamise Microsoft 365 suurettevõtterakendused leiate teemast Office [juurutamise tööriista ülevaade.](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool) Lisateavet selle kohta, kuidas Office kohandamise tööriista kasutada, leiate teemast Office [kohandamise tööriista ülevaade.](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)
