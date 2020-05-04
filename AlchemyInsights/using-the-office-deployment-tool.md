---
title: Office ' i Juurutusriista kasutamine
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: d941bce524dc797d5dcbb7213bded6919fd01b7d
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010860"
---
# <a name="using-the-office-deployment-tool-odt"></a>Office ' i Juurutusriista (ODT) kasutamine

Office ' i juurutamise tööriista (ODT) abil saate juurutada Office 365 Office ' i versiooni. Office ' i juurutamise tööriist (setup. exe) käivitatakse käsurealt ja kasutab konfiguratsiooni XML-faili määratlemaks, milliseid sätteid rakendada Office ' i juurutamisel.
  
1. Laadige alla uusim versioon Office ' i juurutamise tööriist [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Kasutage [Office ' i kohandamisriista (Oct)](https://config.office.com) juurutamise eelistuste valimiseks ja konfiguratsiooni XML-faili loomiseks. Eksportima konfiguratsioonifail ja asetage see kohalikult samasse kausta, kus asub setup. exe.

    **Märkus:** Office ' i installimise probleemid ilmnevad sageli valesti konfigureeritud või vigane konfiguratsioonifailide tõttu. Selliste probleemide vältimiseks soovitame kasutada Office ' i kohandamise tööriista konfiguratsioonifaili loomiseks. Olemasolevaid konfiguratsioonifaile saate importida ka Office ' i Kohandamistööriistasse.

3. Laiendatud käsuviibalt, aktiveerige asukoht, kus setup. exe asub ja käivitage Office ' i juurutamise tööriista allalaadimise režiimis ja määrake äsja salvestatud konfiguratsioonifail. Selles näites konfiguratsioonifaili nimega Configuration. XML:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Käivitage Office ' i juurutamise tööriist Konfigureeri režiimis ja määrake konfiguratsioonifail.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Märkus:** Peate käivitama selle kliendi arvutisse, kuhu soovite Office ' i installida, ja teil peab olema kohaliku administraatori õigused selles arvutis.

Lisateavet Office ' i juurutamise tööriista kasutamise kohta Microsoft 365 rakenduste jaoks ettevõtte juurutamise stsenaariumide puhul vt [Office ' i Juurutustööriista ülevaade](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Office ' i kohandamise tööriista kasutamise kohta lisateabe saamiseks vaadake [Office ' i kohandamise tööriista ülevaade](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
