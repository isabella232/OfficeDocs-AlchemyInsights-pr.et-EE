---
title: Office ' i rakendustele sisselogimisega seotud probleemid
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
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762982"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="becb6-102">Office ' i rakendustele sisselogimisega seotud probleemid</span><span class="sxs-lookup"><span data-stu-id="becb6-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="becb6-103">Office ' i rakendustega sisselogimise probleemide lahendamiseks proovige järgmist.</span><span class="sxs-lookup"><span data-stu-id="becb6-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="becb6-104">Eemaldage kõik töökontod, välja arvatud mõjutatud konto, kasutades Windowsi sätteid > **juurdepääsu töö või kooli**.</span><span class="sxs-lookup"><span data-stu-id="becb6-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="becb6-105">[Tühjendage Office ' i mandaat](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) , kasutades Windowsi mandaat Manager.</span><span class="sxs-lookup"><span data-stu-id="becb6-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="becb6-106">**Märkus:** Office 2016 registri teed on muutunud 16,0.</span><span class="sxs-lookup"><span data-stu-id="becb6-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="becb6-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="becb6-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="becb6-108">Avage Office ' i rakendus, valige **faili** > **konto** > **Logi välja**. Seejärel logige sisse, kasutades kehtivat litsentsi kasutajakontoga.</span><span class="sxs-lookup"><span data-stu-id="becb6-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="becb6-109">Lisateavet vt teemast [Office’i kontod](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="becb6-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="becb6-110">Maci kasutajad võiksid lugeda artiklit [Office 2016 for Maci rakendusse ei saa sisse logida](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="becb6-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="becb6-111">Kui tõrked ilmneb samal ajal, kui ühendate Microsoft 365, kasutades Office 2013, lubage kaasaegne autentimine Office ' i klient.</span><span class="sxs-lookup"><span data-stu-id="becb6-111">If the errors occurs while connecting to Microsoft 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="becb6-112">Lisateavet leiate teemadest</span><span class="sxs-lookup"><span data-stu-id="becb6-112">For more information, see:</span></span>
- [<span data-ttu-id="becb6-113">Te ei saa sisse logida Microsoft 365, Azure või Intune</span><span class="sxs-lookup"><span data-stu-id="becb6-113">You can't sign in to Microsoft 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="becb6-114">Ühenduse probleemid sisselogimise pärast värskenduse Office 2016 ehitada 16.0.7967 Windows 10</span><span class="sxs-lookup"><span data-stu-id="becb6-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="becb6-115">"Kahjuks teine konto teie organisatsioonis on juba sisse logitud selles arvutis" Office</span><span class="sxs-lookup"><span data-stu-id="becb6-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="becb6-116">Sisselogimise probleemide tõrkeotsing Office ' i kaasaegne autentimine ADFS kasutamisel</span><span class="sxs-lookup"><span data-stu-id="becb6-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)