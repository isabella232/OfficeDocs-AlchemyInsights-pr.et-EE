---
title: Küsimused selle kohta, kuidas kasutada Office tööriista (ODT)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: d38866647c7bf286b5b5b21e7fdcc94af72ea1850bc40391af077aa230b8b4fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959679"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Küsimused selle kohta, kuidas kasutada Office tööriista (ODT)

Laadige Office Microsofti allalaadimiskeskusest alla [juurutamise tööriist.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
Pärast faili allalaadimist käivitage iseavanev täitmisfail, mis sisaldab Office juurutustööriista täitmisfaili (setup.exe) ja näidiskonfiguratsioonifaili (configuration.xml).
  
 **Klientarvutitest Microsoft 365 suurettevõtterakendused eemaldamiseks või eemaldamiseks:**
  
Kui installite Microsoft 365 suurettevõtterakendused, saate teatud tooted välistada. Selleks järgige ODT-Office installimise juhiseid, kuid lisage konfiguratsioonifaili element ExcludeApp. Näiteks installib see konfiguratsioonifail kõik Microsoft 365 suurettevõtterakendused peale Publisher.
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Ülevaade Office juurutamise tööriistast](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

