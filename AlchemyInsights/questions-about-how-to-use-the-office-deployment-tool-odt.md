---
title: Küsimustele, kuidas kasutada Office'i juurutamise tööriist (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e91d40f872dd401ee210ac05eb39d64b6fb88027
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371764"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Küsimustele, kuidas kasutada Office'i juurutamise tööriist (ODT)

Office'i juurutamise tööriist alla laadida [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Pärast allalaadimist faili, käivitage iseavanev käivitatava faili, mis sisaldab Office'i juurutamise tööriist käivitatava (setup.exe) ja proovi konfiguratsioonifaili (configuration.xml).
  
 **Või eemaldada Office 365 ProPlus toodete kliendi arvutitega:**
  
Kui installite Office 365 ProPlus, jätta kindlaid tooteid. Selleks järgige juhiseid Office installida selle ODT, kuid sisaldavad ExcludeApp element konfiguratsioonifaili. Näiteks selle konfiguratsiooni faili installib Office 365 ProPlus toodete, välja arvatud Kirjastaja:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Ülevaade Office'i juurutamise tööriist](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

