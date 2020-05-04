---
title: Küsimused Office ' i juurutamise tööriista (ODT) kasutamise kohta
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 4aef42df4dde17d15863fca67e41f0ff23e506dc
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010744"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="90e9c-102">Küsimused Office ' i juurutamise tööriista (ODT) kasutamise kohta</span><span class="sxs-lookup"><span data-stu-id="90e9c-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="90e9c-103">Office ' i juurutamise tööriista alla laadida [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="90e9c-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="90e9c-104">Pärast faili allalaadimist käivitage iseavanev täitmisfail, mis sisaldab Office ' i Juurutustööriista täitmisfaili (setup. exe) ja näidiskonfiguratsioonifaili (Configuration. XML).</span><span class="sxs-lookup"><span data-stu-id="90e9c-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="90e9c-105">**Välistada või eemaldada Microsoft 365 apps ettevõtte toodete klientarvutid:**</span><span class="sxs-lookup"><span data-stu-id="90e9c-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="90e9c-106">Kui installite Microsoft 365 apps Enterprise, saate välistada teatud tooted.</span><span class="sxs-lookup"><span data-stu-id="90e9c-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="90e9c-107">Selleks järgige Office ' i ODT-ga installimiseks juhiseid, kuid lisage konfiguratsioonifailis Excludeappi element.</span><span class="sxs-lookup"><span data-stu-id="90e9c-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="90e9c-108">Näiteks see konfiguratsioonifail installib kõik Microsoft 365 apps ettevõtte toodete peale Publisher:</span><span class="sxs-lookup"><span data-stu-id="90e9c-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="90e9c-109">Office ' i juurutamise tööriista ülevaade</span><span class="sxs-lookup"><span data-stu-id="90e9c-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

