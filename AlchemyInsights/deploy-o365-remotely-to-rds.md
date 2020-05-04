---
title: Juurutamine Microsoft 365 apps ettevõtte ühiskasutuses kasutamiseks RDS, Terminal Server või VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 51512b29f8d37ce6c39ece5bb704cb01e88e463d
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010250"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="6e0c8-102">Juurutamine Microsoft 365 apps ettevõtte ühiskasutuses kasutamiseks RDS, Terminal Server või VDI</span><span class="sxs-lookup"><span data-stu-id="6e0c8-102">Deploying Microsoft 365 Apps for enterprise for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="6e0c8-103">Juurutada Microsoft 365 apps Enterprise kaugtöölaua teenuste (RDS), varem nimega terminaliteenused:</span><span class="sxs-lookup"><span data-stu-id="6e0c8-103">To deploy Microsoft 365 Apps for enterprise using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
- <span data-ttu-id="6e0c8-104">Peab teil olema Microsoft 365 äriplaan või Office 365 kava, mis sisaldab Microsoft 365 apps Enterprise, näiteks Office 365 Enterprise E3 või Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="6e0c8-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE] 
   > <span data-ttu-id="6e0c8-105">Microsoft 365 apps äri ja Microsoft 365 Business Premium Standard plaanid ei sisalda Microsoft 365 apps Enterprise.</span><span class="sxs-lookup"><span data-stu-id="6e0c8-105">The Microsoft 365 Apps for business and Microsoft 365 Business Premium Standard plans do not include Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="6e0c8-106">Peate lubama [ühiskasutatava arvuti aktiveerimise](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="6e0c8-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

> [!NOTE]
> <span data-ttu-id="6e0c8-107">Samuti saate alla laadida ja käivitada [Microsofti toe ja taastamise abimees](https://aka.ms/SaRA_OfficeSCA_M365Portal) installida Microsoft 365 apps Enterprise ühiskasutatava arvuti aktiveerimise režiimis.</span><span class="sxs-lookup"><span data-stu-id="6e0c8-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>

<span data-ttu-id="6e0c8-108">Eeltingimused, setup juhiseid ja juhiseid kohandatud installi Office ' i juurutamise tööriista abil kohta lisateabe saamiseks vaadake [juurutada Microsoft 365 apps Enterprise kaugtöölaua teenuste abil](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="6e0c8-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>

<span data-ttu-id="6e0c8-109">Ühiskasutusega arvuti aktiveerimisega seotud tõrgete lahendamiseks toimige järgmiselt.</span><span class="sxs-lookup"><span data-stu-id="6e0c8-109">To fix errors related to shared computer activation:</span></span>
- <span data-ttu-id="6e0c8-110">Vaadake [tõrkeotsingu probleemid ühiskasutusse antud arvuti aktiveerimine Microsoft 365 apps Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="6e0c8-110">See [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
- <span data-ttu-id="6e0c8-111">Lugege artiklit [Microsoft 365 suurettevõtterakenduste aktiveerimisoleku lähtestamine](https://go.microsoft.com/fwlink/?linkid=2109218) (inglise keeles).</span><span class="sxs-lookup"><span data-stu-id="6e0c8-111">See [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="6e0c8-112">Kui soovite installida Microsoft 365 apps Enterprise RDS Microsoft 365 halduskeskus, ***mis kasutab vaikimisi installi sätted***, toimige järgmiselt:</span><span class="sxs-lookup"><span data-stu-id="6e0c8-112">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1.    <span data-ttu-id="6e0c8-113">Kontrollige, mis tellimus teil on.</span><span class="sxs-lookup"><span data-stu-id="6e0c8-113">Check what subscription you have.</span></span> <span data-ttu-id="6e0c8-114">[Õpi, kuidas](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span><span class="sxs-lookup"><span data-stu-id="6e0c8-114">[Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2.    <span data-ttu-id="6e0c8-115">Vajadusel aktiveerige mõni muu tellimus.</span><span class="sxs-lookup"><span data-stu-id="6e0c8-115">If necessary, switch to a different subscription.</span></span> <span data-ttu-id="6e0c8-116">[Õpi, kuidas](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="6e0c8-116">[Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span></span>
3.    <span data-ttu-id="6e0c8-117">Kui Office on juba installitud RDS-serverisse, kasutades muid Microsofti tellimusi, desinstallige see.</span><span class="sxs-lookup"><span data-stu-id="6e0c8-117">If Office is already installed on the RDS server using any other Microsoft subscriptions, uninstall it.</span></span> <span data-ttu-id="6e0c8-118">Näiteks, **minnes** > juhtpaneeli**desinstallida programmi**.</span><span class="sxs-lookup"><span data-stu-id="6e0c8-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="6e0c8-119">Kui teil on probleeme, desinstallige [Microsofti toe-ja Taasteabimehe](https://aka.ms/SARA-OfficeUninstall-Alchemy) abil.</span><span class="sxs-lookup"><span data-stu-id="6e0c8-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4.    <span data-ttu-id="6e0c8-120">RDS server, logige sisse Microsoft 365 halduskeskus administraatori kontoga ja [installige microsoft 365 apps Enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="6e0c8-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5.    <span data-ttu-id="6e0c8-121">Pärast Office ' i installimist ***Ärge avage ega logige sisse*** ühelegi Office ' i rakendustele.</span><span class="sxs-lookup"><span data-stu-id="6e0c8-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6.    <span data-ttu-id="6e0c8-122">RDS server, lubage ühiskasutusse antud arvuti aktiveerimine registri redigeerimisel toimige järgmiselt:</span><span class="sxs-lookup"><span data-stu-id="6e0c8-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="6e0c8-123">Paremklõpsake ekraani alumises vasakus nurgas asuvat Windowsi nuppu ja valige **Käivita**.</span><span class="sxs-lookup"><span data-stu-id="6e0c8-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="6e0c8-124">Väljale Ava tippige **käsk regedit**ja seejärel valige **OK**.</span><span class="sxs-lookup"><span data-stu-id="6e0c8-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="6e0c8-125">Kui küsitakse, kas Registriredaktor lubab teie seadmes muudatusi teha, valige **Jah** .</span><span class="sxs-lookup"><span data-stu-id="6e0c8-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="6e0c8-126">Registriredaktoris lisada stringi väärtus **Sharedcomputerlicensing** sätte 1 alla HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="6e0c8-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="6e0c8-127">RDS server, logige sisse ***lõppkasutaja*** ja [veenduge, et jagatud arvuti aktiveerimine on lubatud Microsoft 365 apps Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="6e0c8-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

