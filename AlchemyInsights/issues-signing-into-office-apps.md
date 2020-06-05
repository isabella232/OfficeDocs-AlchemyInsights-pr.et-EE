---
title: Probleemid sisselogimisel Microsoft 365 rakendused
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
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579861"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="76ca1-102">Microsoft 365 rakenduste kinnitamine "teie arvuti usaldusväärse platvormi moodul ei tööta korralikult" sõnum</span><span class="sxs-lookup"><span data-stu-id="76ca1-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="76ca1-103">Probleemi lahendamiseks proovige järgmist.</span><span class="sxs-lookup"><span data-stu-id="76ca1-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="76ca1-104">Installige uusimad värskendused [Windowsi](https://support.microsoft.com/help/4027667/windows-10-update) ja [Office ' i](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)jaoks.</span><span class="sxs-lookup"><span data-stu-id="76ca1-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="76ca1-105">[Tühjendage Office ' i mandaat](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) , kasutades Windowsi mandaat Manager.</span><span class="sxs-lookup"><span data-stu-id="76ca1-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="76ca1-106">**Märkus:** Office 2016 registri teed on muutunud 16,0.</span><span class="sxs-lookup"><span data-stu-id="76ca1-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="76ca1-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="76ca1-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="76ca1-108">Proovige [kasutaja taasteprotsessi](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) usaldusväärse platvormi MOODULI (TPM) tõrgete lahendamiseks.</span><span class="sxs-lookup"><span data-stu-id="76ca1-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="76ca1-109">Seadke EnableADAL = 0, kasutades järgmisi samme:</span><span class="sxs-lookup"><span data-stu-id="76ca1-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="76ca1-110">Paremklõpsake Windowsi Start nuppu, valige **Käivita**, tippige **käsk regedit**ja seejärel valige **OK**.</span><span class="sxs-lookup"><span data-stu-id="76ca1-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="76ca1-111">Valige **Jah** , et lubada registriredaktoris teie seadmes muudatusi teha.</span><span class="sxs-lookup"><span data-stu-id="76ca1-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="76ca1-112">Registry Editoris lisada DWORD-väärtus **Enableadal** sätte **0** all HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="76ca1-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="76ca1-113">Lisateabe saamiseks vaadake [ühenduse probleemid sisse logida pärast värskenduse Office 2016 ehitada 16.0.7967 Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="76ca1-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>