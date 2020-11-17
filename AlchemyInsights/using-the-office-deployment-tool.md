---
title: Office ' i juurutamise tööriista kasutamine
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085828"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="22c06-102">Office ' i juurutamise tööriista (ODT) kasutamine</span><span class="sxs-lookup"><span data-stu-id="22c06-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="22c06-103">Office ' i juurutamise tööriista (ODT) abil saate Office ' i 365 Office ' i versioone juurutada.</span><span class="sxs-lookup"><span data-stu-id="22c06-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="22c06-104">Office ' i juurutamise tööriist (setupodt.exe) käivitatakse käsurealt ja see kasutab konfiguratsiooni XML-faili, et määrata, milliseid sätteid Office ' i juurutamisel rakendada.</span><span class="sxs-lookup"><span data-stu-id="22c06-104">The Office Deployment Tool (setupodt.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="22c06-105">Laadige [Microsofti allalaadimiskeskusest](https://go.microsoft.com/fwlink/p/?LinkID=626065)alla Office ' i juurutamise tööriista uusim versioon.</span><span class="sxs-lookup"><span data-stu-id="22c06-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="22c06-106">Kasutage [Office ' i kohandamise tööriista (ÜMT)](https://config.office.com) juurutuse eelistuste valimiseks ja konfiguratsiooni XML-faili loomiseks.</span><span class="sxs-lookup"><span data-stu-id="22c06-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="22c06-107">Eksportige konfiguratsioonifail ja paigutage see lokaalselt samasse kausta, kus asub setupodt.exe.</span><span class="sxs-lookup"><span data-stu-id="22c06-107">Export the configuration file and place it locally on the same folder where the setupodt.exe resides.</span></span>

    <span data-ttu-id="22c06-108">**Märkus:** Office ' i installimisega seotud probleemid ilmnevad sageli valesti konfigureeritud või malformatted konfiguratsioonifailid.</span><span class="sxs-lookup"><span data-stu-id="22c06-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="22c06-109">Selliste probleemide vältimiseks soovitame konfiguratsioonifaili loomiseks kasutada Office ' i kohandamise tööriista.</span><span class="sxs-lookup"><span data-stu-id="22c06-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="22c06-110">Olemasolevaid konfiguratsiooniseadeid saate importida ka Office ' i kohandamise tööriista.</span><span class="sxs-lookup"><span data-stu-id="22c06-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="22c06-111">Liikuge tõstetud käsuviiba kaudu kohale, kus setupodt.exe asub, ja käivitage Office ' i juurutamise tööriist allalaaditavas režiimis ning määrake äsja salvestatud konfiguratsioonifail.</span><span class="sxs-lookup"><span data-stu-id="22c06-111">From an elevated command prompt, switch to the location where setupodt.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="22c06-112">Selles näites on konfiguratsioonifaili nimi Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="22c06-112">In this example, the configuration file is named Configuration.xml:</span></span>

```setupodt.exe /download Configuration.xml```

<span data-ttu-id="22c06-113">4. Käivitage Office ' i juurutamise tööriist konfigureerimise režiimis ja määrake konfiguratsioonifail.</span><span class="sxs-lookup"><span data-stu-id="22c06-113">4.Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>

```setupodt.exe /configure Configuration.xml```

<span data-ttu-id="22c06-114">**Märkus:** Selle toimingu peate käivitama klientarvutis, kuhu soovite Office ' i installida, ja teil peavad olema kohaliku administraatori õigused selles arvutis.</span><span class="sxs-lookup"><span data-stu-id="22c06-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="22c06-115">Lisateavet Office ' i juurutamise tööriista kasutamise kohta Microsoft 365 rakenduste jaoks Enterprise ' i juurutamise stsenaariumide kohta leiate artiklist [Office ' i juurutamise tööriista ülevaade](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="22c06-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="22c06-116">Lisateavet Office ' i kohandamise tööriista kasutamise kohta leiate teemast [Office ' i kohandamise tööriista ülevaade](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="22c06-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
