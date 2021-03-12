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
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709102"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="c3892-102">Microsoft 365 rakenduste parandamine teie arvuti usaldusväärse platvormi moodul ei tööta õigesti "sõnum</span><span class="sxs-lookup"><span data-stu-id="c3892-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="c3892-103">Probleemi lahendamiseks proovige järgmist.</span><span class="sxs-lookup"><span data-stu-id="c3892-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="c3892-104">Installige uusimad värskendused [Windowsile](https://support.microsoft.com/help/4027667/windows-10-update) ja [Office '](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)ile.</span><span class="sxs-lookup"><span data-stu-id="c3892-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="c3892-105">[Tühjendage Office ' i mandaat](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) Windows mandaadi halduri abil.</span><span class="sxs-lookup"><span data-stu-id="c3892-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="c3892-106">**Märkus:** Office 2016 registrite teed on muudetud versiooniks 16,0.</span><span class="sxs-lookup"><span data-stu-id="c3892-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="c3892-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="c3892-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="c3892-108">Proovige lahendada usaldusväärse platvormi mooduli (TPM) tõrked [kasutaja taastamise protsessis](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) .</span><span class="sxs-lookup"><span data-stu-id="c3892-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="c3892-109">Seadke EnableADAL = 0, kasutades järgmisi juhiseid.</span><span class="sxs-lookup"><span data-stu-id="c3892-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="c3892-110">Paremklõpsake Windowsi nuppu Start, valige käsk **Käivita**, tippige **käsk regedit** ja seejärel klõpsake nuppu **OK**.</span><span class="sxs-lookup"><span data-stu-id="c3892-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="c3892-111">Kui soovite, et registriredaktori saaks teie seadmes muudatusi teha, valige **Jah** .</span><span class="sxs-lookup"><span data-stu-id="c3892-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="c3892-112">Registriredaktori korral lisage **ENABLEADAL** DWORD-väärtus, mille sätteks on **0** jaotises HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="c3892-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="c3892-113">Lisateavet leiate teemast [probleemid seoses sisselogimisega pärast Windows 10 versioonile Office 2016 Build 16.0.7967](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="c3892-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>