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
ms.openlocfilehash: c5b055989014b464d3136895702c8ea40e8eb701
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086152"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="03ea0-102">Office ' i juurutamise tööriista (ODT) kasutamise küsimused</span><span class="sxs-lookup"><span data-stu-id="03ea0-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="03ea0-103">Laadige Office ' i juurutamise tööriist alla [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="03ea0-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="03ea0-104">Pärast faili allalaadimist käivitage iseavanev käivitatava faili, mis sisaldab Office ' i juurutamise tööriista täitmisfaili (setupodt.exe) ja proovi konfiguratsioonifaili (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="03ea0-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setupodt.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="03ea0-105">**Klientarvutitest Enterprise ' i toodete Microsoft 365 rakenduste välistamiseks või eemaldamiseks tehke järgmist.**</span><span class="sxs-lookup"><span data-stu-id="03ea0-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="03ea0-106">Kui installite Microsoft 365 rakendusi Enterprise ' ile, saate kindlad tooted välja jätta.</span><span class="sxs-lookup"><span data-stu-id="03ea0-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="03ea0-107">Selleks järgige Office ' i installimisel ODT-s olevaid juhiseid, kuid lisage konfiguratsioonifaili ExcludeApp element.</span><span class="sxs-lookup"><span data-stu-id="03ea0-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="03ea0-108">See konfiguratsioonifail installib näiteks kõik Enterprise ' i toodetele (v. a Publisher) Microsoft 365 rakendused.</span><span class="sxs-lookup"><span data-stu-id="03ea0-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="03ea0-109">Office ' i juurutamise tööriista ülevaade</span><span class="sxs-lookup"><span data-stu-id="03ea0-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

