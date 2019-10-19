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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="f04fe-102">Küsimused Office ' i juurutamise tööriista (ODT) kasutamise kohta</span><span class="sxs-lookup"><span data-stu-id="f04fe-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="f04fe-103">Office ' i juurutamise tööriista alla laadida [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="f04fe-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="f04fe-104">Pärast faili allalaadimist käivitage iseavanev täitmisfail, mis sisaldab Office ' i Juurutustööriista täitmisfaili (setup. exe) ja näidiskonfiguratsioonifaili (Configuration. XML).</span><span class="sxs-lookup"><span data-stu-id="f04fe-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="f04fe-105">**Välistada või eemaldada Office 365 ProPlus toodete klientarvutid:**</span><span class="sxs-lookup"><span data-stu-id="f04fe-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="f04fe-106">Office 365 ProPlus installimisel saate välistada teatud tooted.</span><span class="sxs-lookup"><span data-stu-id="f04fe-106">When installing Office 365 ProPlus, you can exclude specific products.</span></span> <span data-ttu-id="f04fe-107">Selleks järgige Office ' i ODT-ga installimiseks juhiseid, kuid lisage konfiguratsioonifailis Excludeappi element.</span><span class="sxs-lookup"><span data-stu-id="f04fe-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="f04fe-108">Näiteks installib see konfiguratsioonifail kõik Office 365 ProPlusi tooted peale Publisheri:</span><span class="sxs-lookup"><span data-stu-id="f04fe-108">For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="f04fe-109">Office ' i juurutamise tööriista ülevaade</span><span class="sxs-lookup"><span data-stu-id="f04fe-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

