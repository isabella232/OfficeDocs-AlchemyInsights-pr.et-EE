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
ms.openlocfilehash: fa40fef0de9b2e0e1fc329269c24e8bca9ed4146
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726244"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="9ee42-102">Office ' i Juurutusriista (ODT) kasutamine</span><span class="sxs-lookup"><span data-stu-id="9ee42-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="9ee42-103">Office ' i juurutamise tööriista (ODT) abil saate juurutada Office 365 Office ' i versiooni.</span><span class="sxs-lookup"><span data-stu-id="9ee42-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="9ee42-104">Office ' i juurutamise tööriist (setup. exe) käivitatakse käsurealt ja kasutab konfiguratsiooni XML-faili määratlemaks, milliseid sätteid rakendada Office ' i juurutamisel.</span><span class="sxs-lookup"><span data-stu-id="9ee42-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="9ee42-105">Laadige alla uusim versioon Office ' i juurutamise tööriist [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="9ee42-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="9ee42-106">Kasutage [Office ' i kohandamisriista (Oct)](https://config.office.com) juurutamise eelistuste valimiseks ja konfiguratsiooni XML-faili loomiseks.</span><span class="sxs-lookup"><span data-stu-id="9ee42-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="9ee42-107">Eksportima konfiguratsioonifail ja asetage see kohalikult samasse kausta, kus asub setup. exe.</span><span class="sxs-lookup"><span data-stu-id="9ee42-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="9ee42-108">**Märkus:** Office ' i installimise probleemid ilmnevad sageli valesti konfigureeritud või vigane konfiguratsioonifailide tõttu.</span><span class="sxs-lookup"><span data-stu-id="9ee42-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="9ee42-109">Selliste probleemide vältimiseks soovitame kasutada Office ' i kohandamise tööriista konfiguratsioonifaili loomiseks.</span><span class="sxs-lookup"><span data-stu-id="9ee42-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="9ee42-110">Olemasolevaid konfiguratsioonifaile saate importida ka Office ' i Kohandamistööriistasse.</span><span class="sxs-lookup"><span data-stu-id="9ee42-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="9ee42-111">Laiendatud käsuviibalt, aktiveerige asukoht, kus setup. exe asub ja käivitage Office ' i juurutamise tööriista allalaadimise režiimis ja määrake äsja salvestatud konfiguratsioonifail.</span><span class="sxs-lookup"><span data-stu-id="9ee42-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="9ee42-112">Selles näites konfiguratsioonifaili nimega Configuration. XML:</span><span class="sxs-lookup"><span data-stu-id="9ee42-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="9ee42-113">Käivitage Office ' i juurutamise tööriist Konfigureeri režiimis ja määrake konfiguratsioonifail.</span><span class="sxs-lookup"><span data-stu-id="9ee42-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="9ee42-114">**Märkus:** Peate käivitama selle kliendi arvutisse, kuhu soovite Office ' i installida, ja teil peab olema kohaliku administraatori õigused selles arvutis.</span><span class="sxs-lookup"><span data-stu-id="9ee42-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="9ee42-115">Lisateavet Office ' i juurutamise tööriista kasutamise kohta Microsoft 365 rakenduste jaoks ettevõtte juurutamise stsenaariumide puhul vt [Office ' i Juurutustööriista ülevaade](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="9ee42-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span></span> <span data-ttu-id="9ee42-116">Office ' i kohandamise tööriista kasutamise kohta lisateabe saamiseks vaadake [Office ' i kohandamise tööriista ülevaade](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="9ee42-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
