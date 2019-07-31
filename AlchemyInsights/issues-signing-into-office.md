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
- "2574"
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938190"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="90e8e-102">Office apps sisselogimisega probleeme</span><span class="sxs-lookup"><span data-stu-id="90e8e-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="90e8e-103">Office apps sisselogimise probleemide lahendamiseks proovige järgmist:</span><span class="sxs-lookup"><span data-stu-id="90e8e-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="90e8e-104">Eemaldage kõik töö omanikud, välja arvatud mõjutatud konto, kasutades Windowsi sätted > **juurdepääsu tööl või koolis**.</span><span class="sxs-lookup"><span data-stu-id="90e8e-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="90e8e-105">[Selge Office mandaati](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) kasutades Windows Mandaadihaldur.</span><span class="sxs-lookup"><span data-stu-id="90e8e-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="90e8e-106">**Märkus:** Registri teed Office 2016 on muutunud 16,0.</span><span class="sxs-lookup"><span data-stu-id="90e8e-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="90e8e-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="90e8e-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="90e8e-108">Avage mõni Office'i rakendus, valige **faili** > **konto** > **Logi välja**. Seejärel sisse kasutajakontoga, kellel on kehtiv juhiluba.</span><span class="sxs-lookup"><span data-stu-id="90e8e-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="90e8e-109">Üksikasjalikuma teabe saamiseks vt [kontode ametisse](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="90e8e-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="90e8e-110">Mac, vaadake [Office 2016 for Mac app ei saa sisse logida](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="90e8e-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="90e8e-111">Vigade ilmnemisel ühendamisel Office 365, Office 2013 kasutades lubada Office'i kliendi kaasaegne autentimise.</span><span class="sxs-lookup"><span data-stu-id="90e8e-111">If the errors occurs while connecting to Office 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="90e8e-112">Lisateavet vaadake teemast</span><span class="sxs-lookup"><span data-stu-id="90e8e-112">For more information, see:</span></span>
- [<span data-ttu-id="90e8e-113">Te ei saa sisse logida Office 365, Azure ja Intune</span><span class="sxs-lookup"><span data-stu-id="90e8e-113">You can't sign in to Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="90e8e-114">Ühenduse probleemid sisselogimine pärast update Office 2016 ehitada 16.0.7967 Windows 10</span><span class="sxs-lookup"><span data-stu-id="90e8e-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="90e8e-115">"Kahjuks ei õnnestunud teise konto organisatsioonist kirjutatakse juba selles arvutis" asukoht</span><span class="sxs-lookup"><span data-stu-id="90e8e-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="90e8e-116">Tõrkeotsingu sisselogimiseks Office kaasaegne autentimine kui kasutate ADFS</span><span class="sxs-lookup"><span data-stu-id="90e8e-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)