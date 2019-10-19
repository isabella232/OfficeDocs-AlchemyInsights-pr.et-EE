---
title: Küsimused Office ' i juurutamise tööriista (ODT) kasutamise kohta
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 604fc200517316de6e0194bd64e6eb3039cfa61b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36553536"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Küsimused Office ' i juurutamise tööriista (ODT) kasutamise kohta

Office ' i juurutamise tööriista alla laadida [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Pärast faili allalaadimist käivitage iseavanev täitmisfail, mis sisaldab Office ' i Juurutustööriista täitmisfaili (setup. exe) ja näidiskonfiguratsioonifaili (Configuration. XML).
  
 **Välistada või eemaldada Office 365 ProPlus toodete klientarvutid:**
  
Office 365 ProPlus installimisel saate välistada teatud tooted. Selleks järgige Office ' i ODT-ga installimiseks juhiseid, kuid lisage konfiguratsioonifailis Excludeappi element. Näiteks installib see konfiguratsioonifail kõik Office 365 ProPlusi tooted peale Publisheri:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Office ' i juurutamise tööriista ülevaade](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

