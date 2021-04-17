---
title: Microsoft 365 rakendustesse sisselogimisega seotud probleemid
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51832999"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="d974d-102">Microsoft 365 rakenduste parandamine teade "Teie arvuti usaldusväärse platvormi moodul ei tööta õigesti".</span><span class="sxs-lookup"><span data-stu-id="d974d-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="d974d-103">Probleemi lahendamiseks proovige järgmist.</span><span class="sxs-lookup"><span data-stu-id="d974d-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="d974d-104">Installige Windowsi ja [Office'i uusimad](https://support.microsoft.com/help/4027667/windows-10-update) [värskendused.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="d974d-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="d974d-105">[Tühjendage Windowsi identimisteabe](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) halduri abil Office'i identimisteavet.</span><span class="sxs-lookup"><span data-stu-id="d974d-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="d974d-106">**Märkus.** Office 2016 registriteed on muutunud 16.0-ks.</span><span class="sxs-lookup"><span data-stu-id="d974d-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="d974d-107">(Nt: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="d974d-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="d974d-108">Proovige [kasutajataasteprotsessi usaldusväärse](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) platvormi mooduli (TPM) tõrgete lahendamiseks.</span><span class="sxs-lookup"><span data-stu-id="d974d-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="d974d-109">Määrake EnableADAL = 0 järgmiste juhiste abil.</span><span class="sxs-lookup"><span data-stu-id="d974d-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="d974d-110">Paremklõpsake Windowsi nuppu Start, valige **Käivita**, tippige **käsk regedit** ja seejärel valige **OK**.</span><span class="sxs-lookup"><span data-stu-id="d974d-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="d974d-111">Valige **Jah,** et registriredaktor lubaks teie seadmes muudatusi teha.</span><span class="sxs-lookup"><span data-stu-id="d974d-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="d974d-112">Lisage registriredaktoris **EnableADAL-i** DWORD-väärtus sättega **0** jaotises HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="d974d-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="d974d-113">Lisateavet leiate teemast Ühenduseprobleemid sisselogimisel pärast [windows 10 opsüsteemis Office 2016 järgule 16.0.7967 värskendamist.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span><span class="sxs-lookup"><span data-stu-id="d974d-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>