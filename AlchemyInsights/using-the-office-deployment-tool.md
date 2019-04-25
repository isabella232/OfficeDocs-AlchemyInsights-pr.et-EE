---
title: Kasutades Office'i juurutamise tööriist
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: c7e0e96f225030590fdd516eaf3115c93a6335b6
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32423179"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="7fb73-102">Kasutades Office'i juurutamise tööriist (ODT)</span><span class="sxs-lookup"><span data-stu-id="7fb73-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="7fb73-103">Kasutate Office'i juurutamise tööriist (ODT) juurutamine Office 365 versioone Office.</span><span class="sxs-lookup"><span data-stu-id="7fb73-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="7fb73-104">Office'i juurutamise tööriist (setup.exe) on käivitada käsurealt ja konfiguratsiooni XML-faili kasutab milliseid sätteid kohaldada Office'i juurutamisel.</span><span class="sxs-lookup"><span data-stu-id="7fb73-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="7fb73-105">Office'i juurutamise tööriist uusim versioon alla laadida [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="7fb73-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
    
2. <span data-ttu-id="7fb73-106">[Office'i kohandamisriist (OCT)](https://config.office.com) abil juurutamise eelistusi valida ja luua konfiguratsiooni XML-faili.</span><span class="sxs-lookup"><span data-stu-id="7fb73-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="7fb73-107">Konfiguratsiooni faili eksportida ja asetage see kohapeal samasse kausta, kus asub setup.exe.</span><span class="sxs-lookup"><span data-stu-id="7fb73-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span> 
    
    <span data-ttu-id="7fb73-108">**Märkus:** Office'i installi probleemid sageli tekkida et valesti või malformatted failid.</span><span class="sxs-lookup"><span data-stu-id="7fb73-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="7fb73-109">Selliste probleemide vältimiseks soovitame, et kasutate Office'i kohandamise tööriista loomiseks konfiguratsioonifaili.</span><span class="sxs-lookup"><span data-stu-id="7fb73-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="7fb73-110">Olemasolevad failid saate importida ka Office'i kohandamise tööriista.</span><span class="sxs-lookup"><span data-stu-id="7fb73-110">You can also import existing configuration files into the Office Customization Tool.</span></span> 
    
3. <span data-ttu-id="7fb73-111">Alates tõstetud käsuviipa, kus elab setup.exe asukohta vahetada ja käivitage Office'i juurutamise tööriist laadida mode ja määrake salvestatud konfiguratsiooni fail.</span><span class="sxs-lookup"><span data-stu-id="7fb73-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="7fb73-112">Selles näites konfiguratsiooni faili nimi Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="7fb73-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="7fb73-113">Käivitage Office'i juurutamise tööriist konfigureerida režiimis ja määrake konfiguratsioonifaili.</span><span class="sxs-lookup"><span data-stu-id="7fb73-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="7fb73-114">**Märkus:** Käivitate kliendi arvutisse, kuhu soovite Office'i installida ja peavad olema kohaliku administraatori õigused, et selle sammu.</span><span class="sxs-lookup"><span data-stu-id="7fb73-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span> 
    
<span data-ttu-id="7fb73-115">Kasutades Office'i juurutamise tööriist teie Office 365 ProPlus juurutamise stsenaariumide kohta lisateabe saamiseks vaadake [Office'i juurutamise tööriist ülevaade](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="7fb73-115">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span></span> <span data-ttu-id="7fb73-116">Office'i kohandamise tööriista kasutamise kohta lisateabe saamiseks vaadake [Office'i kohandamise tööriista ülevaade](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="7fb73-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
  

