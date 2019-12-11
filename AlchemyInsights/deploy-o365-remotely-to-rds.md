---
title: Juurutamine Office 365 ProPlus ühiskasutuses kasutamiseks RDS, Terminal Server või VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959456"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="4f36b-102">Juurutamine Office 365 ProPlus ühiskasutuses kasutamiseks RDS, Terminal Server või VDI</span><span class="sxs-lookup"><span data-stu-id="4f36b-102">Deploying Office 365 ProPlus for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="4f36b-103">Office 365 ProPlusi juurutamine kaugtöölaua teenuste (RDS), varem nimega Terminal Services abil:</span><span class="sxs-lookup"><span data-stu-id="4f36b-103">To deploy Office 365 ProPlus using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
- <span data-ttu-id="4f36b-104">Peab teil olema Microsoft 365 äriplaan või Office 365 kava, mis sisaldab Office 365 ProPlus, näiteks Office 365 Enterprise E3 või Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="4f36b-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE] 
   > <span data-ttu-id="4f36b-105">Office 365 Business ja Office 365 Business Premiumi plaanid ei sisalda Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="4f36b-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
- <span data-ttu-id="4f36b-106">Peate lubama [ühiskasutatava arvuti aktiveerimise](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="4f36b-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

> [!NOTE]
> <span data-ttu-id="4f36b-107">Samuti saate alla laadida ja käivitada [Microsoft support ja taastamise abimees](https://aka.ms/SaRA_OfficeSCA_M365Portal) installida Office 365 ProPlus jagatud arvuti aktiveerimise režiimis.</span><span class="sxs-lookup"><span data-stu-id="4f36b-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>

<span data-ttu-id="4f36b-108">Eeltingimused, setup juhiseid ja juhiseid kohandatud installi Office ' i juurutamise tööriista abil kohta lisateabe saamiseks vaadake [juurutamine office 365 ProPlus kaugtöölaua teenuste abil](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="4f36b-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>

<span data-ttu-id="4f36b-109">Ühiskasutusega arvuti aktiveerimisega seotud tõrgete lahendamiseks toimige järgmiselt.</span><span class="sxs-lookup"><span data-stu-id="4f36b-109">To fix errors related to shared computer activation:</span></span>
- <span data-ttu-id="4f36b-110">Vaadake [tõrkeotsingu probleemid ühiskasutusse antud arvuti aktiveerimine Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="4f36b-110">See [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
- <span data-ttu-id="4f36b-111">Vt [Lähtesta Office 365 ProPlus aktiveerimise olek](https://go.microsoft.com/fwlink/?linkid=2109218).</span><span class="sxs-lookup"><span data-stu-id="4f36b-111">See [Reset Office 365 ProPlus activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="4f36b-112">Kui soovite installida Office 365 ProPlus RDS Microsoft 365 halduskeskus, ***mis kasutab vaikimisi installi sätted***, toimige järgmiselt:</span><span class="sxs-lookup"><span data-stu-id="4f36b-112">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1.  <span data-ttu-id="4f36b-113">Kontrollige, milline Office 365 plaan teil on.</span><span class="sxs-lookup"><span data-stu-id="4f36b-113">Check what Office 365 plan you have.</span></span> <span data-ttu-id="4f36b-114">[Õpi, kuidas](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span><span class="sxs-lookup"><span data-stu-id="4f36b-114">[Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2.  <span data-ttu-id="4f36b-115">Vajadusel aktiveerige mõni muu Office 365 plaan.</span><span class="sxs-lookup"><span data-stu-id="4f36b-115">If necessary, switch to a different Office 365 plan.</span></span> <span data-ttu-id="4f36b-116">[Õpi, kuidas](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="4f36b-116">[Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span></span>
3.  <span data-ttu-id="4f36b-117">Kui Office on juba installitud RDS server, kasutades muid Office 365 plaanid, desinstallige see.</span><span class="sxs-lookup"><span data-stu-id="4f36b-117">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="4f36b-118">Näiteks, **minnes** > juhtpaneeli**desinstallida programmi**.</span><span class="sxs-lookup"><span data-stu-id="4f36b-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="4f36b-119">Kui teil on probleeme, desinstallige [Microsofti toe-ja Taasteabimehe](https://aka.ms/SARA-OfficeUninstall-Alchemy) abil.</span><span class="sxs-lookup"><span data-stu-id="4f36b-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4.  <span data-ttu-id="4f36b-120">RDS server, logige sisse Microsoft 365 halduskeskus administraatori kontoga ja [installige Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="4f36b-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5.  <span data-ttu-id="4f36b-121">Pärast Office ' i installimist ***Ärge avage ega logige sisse*** ühelegi Office ' i rakendustele.</span><span class="sxs-lookup"><span data-stu-id="4f36b-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6.  <span data-ttu-id="4f36b-122">RDS server, lubage ühiskasutusse antud arvuti aktiveerimine registri redigeerimisel toimige järgmiselt:</span><span class="sxs-lookup"><span data-stu-id="4f36b-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="4f36b-123">Paremklõpsake ekraani alumises vasakus nurgas asuvat Windowsi nuppu ja valige **Käivita**.</span><span class="sxs-lookup"><span data-stu-id="4f36b-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="4f36b-124">Väljale Ava tippige **käsk regedit**ja seejärel valige **OK**.</span><span class="sxs-lookup"><span data-stu-id="4f36b-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="4f36b-125">Kui küsitakse, kas Registriredaktor lubab teie seadmes muudatusi teha, valige **Jah** .</span><span class="sxs-lookup"><span data-stu-id="4f36b-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="4f36b-126">Registriredaktoris lisada stringi väärtus **Sharedcomputerlicensing** sätte 1 alla HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="4f36b-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="4f36b-127">RDS server, logige sisse ***lõppkasutaja*** ja [veenduge, et ühiskasutuses arvuti aktiveerimine on lubatud Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="4f36b-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

