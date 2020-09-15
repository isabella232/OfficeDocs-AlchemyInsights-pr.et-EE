---
title: Office ' i installimine terminaliserveri – litsentsimata
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663113"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="9d3a7-102">Office ' i installimine terminaliserveri</span><span class="sxs-lookup"><span data-stu-id="9d3a7-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="9d3a7-103">Rakenduse Microsoft 365 for Enterprise for Enterprise Windowsi serverile juurutamiseks kaugtöölaua teenuste (RDS), varem nimega terminaliteenuste kaudu.</span><span class="sxs-lookup"><span data-stu-id="9d3a7-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="9d3a7-104">Teil peab olema Microsoft 365 tellimus, mis sisaldab Enterprise ' i jaoks mõeldud Microsoft 365 rakendusi (nt Office 365 Enterprise E3 või Enterprise E5).</span><span class="sxs-lookup"><span data-stu-id="9d3a7-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="9d3a7-105">Microsoft 365 rakendused ettevõtetele ja Microsoft 365 for Premiumi lepingud ei sisalda Microsoft 365 Enterprise ' i jaoks mõeldud rakendusi.</span><span class="sxs-lookup"><span data-stu-id="9d3a7-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="9d3a7-106">Peate lubama [ühiskasutatava arvuti aktiveerimise](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="9d3a7-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="9d3a7-107">Kui soovite installida Microsoft 365 rakendusi RDS-ile Microsoft 365 halduskeskus, ***mis kasutab vaikimisi installi sätteid***, kasutage järgmisi juhiseid.</span><span class="sxs-lookup"><span data-stu-id="9d3a7-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="9d3a7-108">Samuti saate alla laadida ja käivitada [Microsofti tugiteenuste ja taastekonsooli abilise](https://aka.ms/SaRA_OfficeSCA_M365Portal) , et installida Office ' i ühiskasutusega arvuti aktiveerimise režiimis Microsoft 365 rakendused.</span><span class="sxs-lookup"><span data-stu-id="9d3a7-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="9d3a7-109">Vaadake, milline Microsoft 365 tellimus teil on.</span><span class="sxs-lookup"><span data-stu-id="9d3a7-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="9d3a7-110">Uurige, kuidas</span><span class="sxs-lookup"><span data-stu-id="9d3a7-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="9d3a7-111">Vajadusel aktiveerige mõni muu Microsoft 365 tellimus.</span><span class="sxs-lookup"><span data-stu-id="9d3a7-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="9d3a7-112">Uurige, kuidas</span><span class="sxs-lookup"><span data-stu-id="9d3a7-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="9d3a7-113">Kui Office on juba RDS-serverisse installitud mis tahes muu Microsoft 365 tellimuse abil, desinstallige see.</span><span class="sxs-lookup"><span data-stu-id="9d3a7-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="9d3a7-114">Näiteks juhtpaneeli käsuga \> Desinstalli programm.</span><span class="sxs-lookup"><span data-stu-id="9d3a7-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="9d3a7-115">Kui teil on probleeme, desinstallige [Microsoft support ja Recovery Assistanti](https://aka.ms/SARA-OfficeUninstall-Alchemy) abil.</span><span class="sxs-lookup"><span data-stu-id="9d3a7-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="9d3a7-116">Rakenduses RDS logige sisse oma administraatori kontoga Microsoft 365 halduskeskus ja [installige Enterprise ' i jaoks microsoft 365](https://portal.office.com/OLS/MySoftware.aspx)' i rakendused.</span><span class="sxs-lookup"><span data-stu-id="9d3a7-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="9d3a7-117">Kui Office on installitud, ***Ärge avage ega logige sisse*** ühtegi Office ' i rakendusse.</span><span class="sxs-lookup"><span data-stu-id="9d3a7-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="9d3a7-118">RDS-serveris lubage ühiskasutusega arvuti aktiveerimine, redigeerides registrit, järgides järgmisi juhiseid.</span><span class="sxs-lookup"><span data-stu-id="9d3a7-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="9d3a7-119">Paremklõpsake ekraani vasakus allnurgas olevat nuppu Windows ja valige Käivita.</span><span class="sxs-lookup"><span data-stu-id="9d3a7-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="9d3a7-120">Tippige väljale Ava **käsk regedit**ja seejärel klõpsake nuppu OK.</span><span class="sxs-lookup"><span data-stu-id="9d3a7-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="9d3a7-121">Kui teilt küsitakse, kas soovite, et registriredaktori saaks teie seadmes muudatusi teha, valige Jah.</span><span class="sxs-lookup"><span data-stu-id="9d3a7-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="9d3a7-122">Lisage registriredaktori **SharedComputerLicensing** stringi väärtus, mille sätteks on HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="9d3a7-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="9d3a7-123">RDS-serveris ***logige sisse lõppkasutajana*** ja veenduge, [et ühiskasutusega arvuti aktiveerimine oleks lubatud Microsoft 365 rakenduste jaoks Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)' i jaoks.</span><span class="sxs-lookup"><span data-stu-id="9d3a7-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="9d3a7-124">Lisateavet Office ' i juurutamise tööriista funktsioonide, häälestamise juhiste ja kohandatud installide juhiste kohta leiate teemast Office ' i juurutamise tööriista kasutamine rakenduses [Microsoft 365 Apps for Enterprise kaugtöölaua teenuste abil](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="9d3a7-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="9d3a7-125">Ühiskasutusega arvuti aktiveerimisega seotud tõrgete lahendamiseks lugege teemat [ühiskasutusega arvuti aktiveerimisega seotud probleemide tõrkeotsing Enterprise ' i jaoks mõeldud Microsoft 365 rakenduste jaoks](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="9d3a7-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  