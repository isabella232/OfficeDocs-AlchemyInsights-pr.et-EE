---
title: Kasutades Office'i juurutamise tööriist
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: b4ade0f21794a8986aa7a37d783da5fa289488fc
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29466269"
---
# <a name="using-the-office-deployment-tool-odt"></a>Kasutades Office'i juurutamise tööriist (ODT)

Kasutate Office'i juurutamise tööriist (ODT) juurutamine Office 365 versioone Office. Office'i juurutamise tööriist (setup.exe) on käivitada käsurealt ja konfiguratsiooni XML-faili kasutab milliseid sätteid kohaldada Office'i juurutamisel.
  
1. Office'i juurutamise tööriist uusim versioon alla laadida [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).
    
2. [Office'i kohandamisriist (OCT)](https://config.office.com) abil juurutamise eelistusi valida ja luua konfiguratsiooni XML-faili. Konfiguratsiooni faili eksportida ja asetage see kohapeal samasse kausta, kus asub setup.exe. 
    
    **Märkus:** Office'i installi probleemid sageli tekkida et valesti või malformatted failid. Selliste probleemide vältimiseks soovitame, et kasutate Office'i kohandamise tööriista loomiseks konfiguratsioonifaili. Olemasolevad failid saate importida ka Office'i kohandamise tööriista. 
    
3. Alates tõstetud käsuviipa, kus elab setup.exe asukohta vahetada ja käivitage Office'i juurutamise tööriist laadida mode ja määrake salvestatud konfiguratsiooni fail. Selles näites konfiguratsiooni faili nimi Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Käivitage Office'i juurutamise tööriist konfigureerida režiimis ja määrake konfiguratsioonifaili.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Märkus:** Käivitate kliendi arvutisse, kuhu soovite Office'i installida ja peavad olema kohaliku administraatori õigused, et selle sammu. 
    
Kasutades Office'i juurutamise tööriist teie Office 365 ProPlus juurutamise stsenaariumide kohta lisateabe saamiseks vaadake [Office'i juurutamise tööriist ülevaade](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Office'i kohandamise tööriista kasutamise kohta lisateabe saamiseks vaadake [Office'i kohandamise tööriista ülevaade](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
  

