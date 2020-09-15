---
title: Microsoft 365 rakendustesse sisselogimisega seotud probleemid
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695283"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="478b0-102">Tühi sisselogimiskuva Microsoft 365 rakendustes</span><span class="sxs-lookup"><span data-stu-id="478b0-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="478b0-103">Probleemi lahendamiseks proovige teha järgmist.</span><span class="sxs-lookup"><span data-stu-id="478b0-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="478b0-104">Installige uusimad värskendused [Windowsile](https://support.microsoft.com/help/4027667/windows-10-update) ja [Office '](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)ile.</span><span class="sxs-lookup"><span data-stu-id="478b0-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="478b0-105">Internet Exploreri suvandite lähtestamine: valige **Tööriistad**  >  **Interneti-suvandid**  >  **täiustatud**  >  **lähtestage Internet Exploreri sätted** (Pange tähele, et te kaotate kohandatud sätted) ja proovige siis uuesti Office ' isse sisse logida.</span><span class="sxs-lookup"><span data-stu-id="478b0-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="478b0-106">Keelake Windows Defender Application Guard (WDAG) või mõni muu sarnane tulemüür või viirusetõrje programm.</span><span class="sxs-lookup"><span data-stu-id="478b0-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="478b0-107">Avage juhtpaneelil jaotis **programmid**ja seejärel valige Windowsi funktsioonide sisse- **või väljalülitamine**.</span><span class="sxs-lookup"><span data-stu-id="478b0-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="478b0-108">Kui Windows Defenderi rakenduse valvur on lubatud, proovige see keelata.</span><span class="sxs-lookup"><span data-stu-id="478b0-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="478b0-109">**Märkus:** Võimalik, et peate arvuti taaskäivitama.</span><span class="sxs-lookup"><span data-stu-id="478b0-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="478b0-110">Veenduge, et rakenduse või tulemüüri/viirusetõrje programm ei blokeeriks Microsoft. AAD. BrokerPlugin [AAD WAM lisandmoodulit](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) .</span><span class="sxs-lookup"><span data-stu-id="478b0-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="478b0-111">[Tühjendage Office ' i mandaat](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows mandaadi halduri abil.</span><span class="sxs-lookup"><span data-stu-id="478b0-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="478b0-112">**Märkus:** Office 2016 registrite teed on muudetud versiooniks 16,0.</span><span class="sxs-lookup"><span data-stu-id="478b0-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="478b0-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="478b0-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="478b0-114">Lisateavet leiate teemast [probleemid seoses sisselogimisega pärast Windows 10 versioonile Office 2016 Build 16.0.7967](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="478b0-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>