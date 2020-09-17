---
title: Office ' i juurutamise tööriista (ODT) kasutamise küsimused
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e9f7581fd21cf5ca2d712038c4b73b67d08f3a76
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774887"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Office ' i juurutamise tööriista (ODT) kasutamise küsimused

Laadige Office ' i juurutamise tööriist alla [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Pärast faili allalaadimist käivitage iseavanev käivitatava faili, mis sisaldab Office ' i juurutamise tööriista täitmisfaili (setup.exe) ja proovi konfiguratsioonifaili (configuration.xml).
  
 **Klientarvutitest Enterprise ' i toodete Microsoft 365 rakenduste välistamiseks või eemaldamiseks tehke järgmist.**
  
Kui installite Microsoft 365 rakendusi Enterprise ' ile, saate kindlad tooted välja jätta. Selleks järgige Office ' i installimisel ODT-s olevaid juhiseid, kuid lisage konfiguratsioonifaili ExcludeApp element. See konfiguratsioonifail installib näiteks kõik Enterprise ' i toodetele (v. a Publisher) Microsoft 365 rakendused.
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Office ' i juurutamise tööriista ülevaade](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

