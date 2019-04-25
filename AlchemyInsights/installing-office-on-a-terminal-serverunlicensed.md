---
title: Paigaldus office Terminal Server - litsentseerimata
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 971edd9c064b448446ba16361e99df4a2291c14f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32410118"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="0bf14-102">Paigaldus Office terminali Server</span><span class="sxs-lookup"><span data-stu-id="0bf14-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="0bf14-103">Kohta Office 365 ProPlusi kasutades kaugtöölaua teenuste (RDS) server Windowsi, endise nimega terminaliteenused:</span><span class="sxs-lookup"><span data-stu-id="0bf14-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="0bf14-104">Peab teil olema Office 365 leping, mis sisaldab Office 365 ProPlus, Office 365 Enterprise E3 või Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="0bf14-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="0bf14-105">Office 365 Business ja Office 365 Business Premium lepingute ei sisalda Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="0bf14-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
    
- <span data-ttu-id="0bf14-106">Peate lubama [ühiskasutatavas arvutis aktiveerimisega](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="0bf14-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>
    
<span data-ttu-id="0bf14-107">Kui soovite installida Office 365 ProPlus RDS portaalist Office 365, \*\* *mis kasutab vaikimisi installimise sätted* \*\*, järgige neid samme:</span><span class="sxs-lookup"><span data-stu-id="0bf14-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, \*\* *which uses default installation settings* \*\*, follow these steps:</span></span> 
  
1. <span data-ttu-id="0bf14-108">Vaata mida teil Office 365 leping.</span><span class="sxs-lookup"><span data-stu-id="0bf14-108">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="0bf14-109">Õppida, kuidas</span><span class="sxs-lookup"><span data-stu-id="0bf14-109">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. <span data-ttu-id="0bf14-110">Kui lüliti erinevate Office 365 korral.</span><span class="sxs-lookup"><span data-stu-id="0bf14-110">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="0bf14-111">Õppida, kuidas</span><span class="sxs-lookup"><span data-stu-id="0bf14-111">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. <span data-ttu-id="0bf14-112">Kui Office on juba installitud, kasutades Office 365 lepingud RDS server, eemaldage see.</span><span class="sxs-lookup"><span data-stu-id="0bf14-112">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="0bf14-113">Näiteks minnes juhtpaneelil \> programmi desinstallimine.</span><span class="sxs-lookup"><span data-stu-id="0bf14-113">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="0bf14-114">Desinstallige [Microsoft Support ja taastamise abimees](https://aka.ms/SARA-OfficeUninstall-Alchemy) kui teil tekib küsimusi.</span><span class="sxs-lookup"><span data-stu-id="0bf14-114">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span> 
    
4. <span data-ttu-id="0bf14-115">RDS server, logige sisse Office 365 portaali administraatori kontoga ja [installige Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="0bf14-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
    
5. <span data-ttu-id="0bf14-116">Pärast Office'i installimist \*\* *Ärge avage või logige sisse* \*\* et kõik Office'i rakendused.</span><span class="sxs-lookup"><span data-stu-id="0bf14-116">After Office is installed, \*\* *don't open or sign in* \*\* to any Office applications.</span></span> 
    
6. <span data-ttu-id="0bf14-117">RDS server, luba ühiskasutatavas arvutis aktiveerimisega redigeerige registrit järgmiselt:</span><span class="sxs-lookup"><span data-stu-id="0bf14-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
    
1. <span data-ttu-id="0bf14-118">Ekraani alumises vasakus nurgas nuppu Windows paremklõpsake ja valige käsk Käivita.</span><span class="sxs-lookup"><span data-stu-id="0bf14-118">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="0bf14-119">Väljale Ava **tippigeregedit**, ja seejärel klõpsake nuppu OK.</span><span class="sxs-lookup"><span data-stu-id="0bf14-119">In the Open box, type **regedit**, and then select OK.</span></span> 
    
2. <span data-ttu-id="0bf14-120">Valige Jah kui teil palutakse Registry Editor võimaldab muuta seadme.</span><span class="sxs-lookup"><span data-stu-id="0bf14-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>
    
3. <span data-ttu-id="0bf14-121">Registry Editor, lisage string väärtus **SharedComputerLicensing** säte on HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration 1.</span><span class="sxs-lookup"><span data-stu-id="0bf14-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span> 
    
7. <span data-ttu-id="0bf14-122">RDS server \*\* *lõppkasutajad sisselogimise* \*\* ja [ühiskasutatavas arvutis aktiveerimisega on lubatud jaoks Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="0bf14-122">On the RDS server, \*\* *sign in as an end user* \*\* and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>
    
<span data-ttu-id="0bf14-123">Eeltingimused, juhiseid ja suuniseid kohandatud installide kasutate Office'i juurutamise tööriist üksikasjalikumalt, vt [Juurutamine Office 365 ProPlusi kasutades kaugtöölaua teenused](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="0bf14-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="0bf14-124">Ühiskasutatavas arvutis aktiveerimisega seotud tõrgete lahendamiseks vaadake [tõrkeotsing küsimusi ühiskasutatavas arvutis aktiveerimisega jaoks Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="0bf14-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  

