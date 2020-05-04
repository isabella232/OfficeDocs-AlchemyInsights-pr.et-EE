---
title: Office ' i installimine terminaliserverisse-litsentsimata
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 6e952513679c9ac66f8de2b43d6d243cf17ff789
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010610"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="17957-102">Office ' i installimine terminaliserverisse</span><span class="sxs-lookup"><span data-stu-id="17957-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="17957-103">Juurutamiseks Microsoft 365 apps Enterprise Windows Server kaugtöölaua teenuste (RDS), varem nimega Terminal Services kasutamisel:</span><span class="sxs-lookup"><span data-stu-id="17957-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="17957-104">Teil peab olema Microsoft 365 tellimus, mis sisaldab Microsoft 365 apps Enterprise, nt Office 365 Enterprise E3 või Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="17957-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="17957-105">Microsoft 365 apps äri ja Microsoft 365 apps Business Premium plaanid ei sisalda Microsoft 365 apps Enterprise.</span><span class="sxs-lookup"><span data-stu-id="17957-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="17957-106">Peate lubama [ühiskasutusega arvuti aktiveerimise](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="17957-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="17957-107">Kui soovite installida Microsoft 365 apps Enterprise RDS Microsoft 365 halduskeskus, ***mis kasutab vaikimisi installi sätted***, kasutage järgmisi samme.</span><span class="sxs-lookup"><span data-stu-id="17957-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="17957-108">Samuti saate alla laadida ja käivitada [Microsofti toe ja taastamise abimees](https://aka.ms/SaRA_OfficeSCA_M365Portal) installida Microsoft 365 apps Enterprise ühiskasutatava arvuti aktiveerimise režiimis.</span><span class="sxs-lookup"><span data-stu-id="17957-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="17957-109">Kontrollige, mida Microsoft 365 tellimus teil on.</span><span class="sxs-lookup"><span data-stu-id="17957-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="17957-110">Vaadake, kuidas</span><span class="sxs-lookup"><span data-stu-id="17957-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="17957-111">Vajadusel aktiveerige mõni muu Microsoft 365 tellimus.</span><span class="sxs-lookup"><span data-stu-id="17957-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="17957-112">Vaadake, kuidas</span><span class="sxs-lookup"><span data-stu-id="17957-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="17957-113">Kui Office on juba installitud RDS server, kasutades muid Microsoft 365 tellimused, desinstallige see.</span><span class="sxs-lookup"><span data-stu-id="17957-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="17957-114">Näiteks, minnes juhtpaneeli \> desinstallida programmi.</span><span class="sxs-lookup"><span data-stu-id="17957-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="17957-115">Kui teil on probleeme, desinstallige [Microsofti toe-ja Taasteabimehe](https://aka.ms/SARA-OfficeUninstall-Alchemy) abil.</span><span class="sxs-lookup"><span data-stu-id="17957-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="17957-116">RDS server, logige sisse Microsoft 365 halduskeskus administraatori kontoga ja [installige microsoft 365 apps Enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="17957-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="17957-117">Pärast Office ' i installimist ***Ärge avage ega logige sisse*** ühelegi Office ' i rakendustele.</span><span class="sxs-lookup"><span data-stu-id="17957-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="17957-118">RDS server, lubage ühiskasutusse antud arvuti aktiveerimine registri redigeerimisel toimige järgmiselt:</span><span class="sxs-lookup"><span data-stu-id="17957-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="17957-119">Paremklõpsake ekraani alumises vasakus nurgas asuvat Windowsi nuppu ja valige käsk Käivita.</span><span class="sxs-lookup"><span data-stu-id="17957-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="17957-120">Väljale Ava tippige **käsk regedit**ja seejärel valige OK.</span><span class="sxs-lookup"><span data-stu-id="17957-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="17957-121">Kui küsitakse, kas Registriredaktor lubab teie seadmes muudatusi teha, valige Jah.</span><span class="sxs-lookup"><span data-stu-id="17957-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="17957-122">Registriredaktoris lisada stringi väärtus **Sharedcomputerlicensing** sätte 1 alla HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="17957-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="17957-123">RDS server, logige sisse ***lõppkasutaja*** ja [veenduge, et jagatud arvuti aktiveerimine on lubatud Microsoft 365 apps Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="17957-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="17957-124">Eeltingimused, setup juhiseid ja juhiseid kohandatud installi Office ' i juurutamise tööriista abil kohta lisateabe saamiseks lugege [juurutada Microsoft 365 apps Enterprise kaugtöölaua teenuste abil](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="17957-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="17957-125">Ühiskasutatava arvuti aktiveerimisega seotud tõrgete lahendamiseks vaadake teemat [microsofti 365 rakenduste jaoks ühiskasutatava arvuti aktiveerimise tõrkeotsing](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="17957-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  