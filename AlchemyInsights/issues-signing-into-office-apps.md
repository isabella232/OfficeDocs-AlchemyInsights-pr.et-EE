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
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938192"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="958ef-102">Office'i rakendused "arvuti usaldusväärse platvormi moodul ei tööta korralikult" sõnumi kinnitamine</span><span class="sxs-lookup"><span data-stu-id="958ef-102">Fixing the Office apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="958ef-103">Probleemi lahendamiseks proovige järgmist:</span><span class="sxs-lookup"><span data-stu-id="958ef-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="958ef-104">Installige uusimad värskendused [Windowsile](https://support.microsoft.com/help/4027667/windows-10-update) ja [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="958ef-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="958ef-105">[Selge Office mandaati](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) kasutades Windows Mandaadihaldur.</span><span class="sxs-lookup"><span data-stu-id="958ef-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="958ef-106">**Märkus:** Registri teed Office 2016 on muutunud 16,0.</span><span class="sxs-lookup"><span data-stu-id="958ef-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="958ef-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="958ef-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="958ef-108">Proovige [kasutaja taastamise protsess](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) määrata usaldusväärse platvormi mooduli (TPM) ebaõnnestumisi.</span><span class="sxs-lookup"><span data-stu-id="958ef-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="958ef-109">Määra ning EnableADAL = 0, tehes järgmist:</span><span class="sxs-lookup"><span data-stu-id="958ef-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="958ef-110">Paremklõpsake Windowsi nuppu Start, valige **Käivita**, tippige **käsk regedit**ja seejärel klõpsake **nuppu OK**.</span><span class="sxs-lookup"><span data-stu-id="958ef-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="958ef-111">Valige **Jah** registriredaktori abil muuta seadme lubamiseks.</span><span class="sxs-lookup"><span data-stu-id="958ef-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="958ef-112">Registriredaktoris lisada säte **0** all HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity on **EnableADAL** DWORD-väärtus.</span><span class="sxs-lookup"><span data-stu-id="958ef-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="958ef-113">Vaadake lisateavet jaotisest [ühenduse küsimusi sisselogimine pärast update Office 2016 ehitada 16.0.7967 Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="958ef-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>