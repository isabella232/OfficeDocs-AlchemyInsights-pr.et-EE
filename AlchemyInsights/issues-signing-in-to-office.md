---
title: Office apps sisselogimisega probleeme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938191"
---
# <a name="blank-sign-in-screen-in-office-apps"></a><span data-ttu-id="c38a9-102">Tühi sisselogimiskuva Office'i rakendustes</span><span class="sxs-lookup"><span data-stu-id="c38a9-102">Blank sign-in screen in Office apps</span></span>

<span data-ttu-id="c38a9-103">Selle probleemi lahendamiseks proovige järgmist:</span><span class="sxs-lookup"><span data-stu-id="c38a9-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="c38a9-104">Installige uusimad värskendused [Windowsile](https://support.microsoft.com/help/4027667/windows-10-update) ja [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="c38a9-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="c38a9-105">Lähtesta Internet Explorer valikud: valige **Tööriistad** > **Interneti-suvandid** > **Täpsemalt** > **Internet Exploreri sätete lähtestamine** (Pange tähele, et te kaotate kohandatud sätted) ning proovige uuesti sisse logida Office.</span><span class="sxs-lookup"><span data-stu-id="c38a9-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="c38a9-106">Keelake Windows Defender taotluse valvur (WDAG) või muud sarnast tulemüür või viirusetõrje programmi.</span><span class="sxs-lookup"><span data-stu-id="c38a9-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="c38a9-107">Juhtpaneelil, minge **programmid**ja valige **Windowsi funktsioonide sisse- või väljalülitamine**.</span><span class="sxs-lookup"><span data-stu-id="c38a9-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="c38a9-108">Kui Windows Defender taotluse Guard on lubatud, keelake see.</span><span class="sxs-lookup"><span data-stu-id="c38a9-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="c38a9-109">**Märkus:** Peate arvuti taaskäivitama.</span><span class="sxs-lookup"><span data-stu-id="c38a9-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="c38a9-110">Tagada, et Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ei taotluse või tulemüüri/anti-Anti-Virus programm poolt blokeeritud.</span><span class="sxs-lookup"><span data-stu-id="c38a9-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="c38a9-111">[Selge Office mandaati](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) kasutades Windows Mandaadihaldur.</span><span class="sxs-lookup"><span data-stu-id="c38a9-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="c38a9-112">**Märkus:** Registri teed Office 2016 on muutunud 16,0.</span><span class="sxs-lookup"><span data-stu-id="c38a9-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="c38a9-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="c38a9-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="c38a9-114">Vaadake lisateavet jaotisest [ühenduse küsimusi sisselogimine pärast update Office 2016 ehitada 16.0.7967 Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="c38a9-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>