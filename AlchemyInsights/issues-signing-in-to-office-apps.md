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
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695319"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="97c9c-102">Microsoft 365 rakenduste parandamine "Kahjuks on teie ettevõtte teine konto juba sisse logitud" sõnumis</span><span class="sxs-lookup"><span data-stu-id="97c9c-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="97c9c-103">Probleemi lahendamiseks proovige järgmist.</span><span class="sxs-lookup"><span data-stu-id="97c9c-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="97c9c-104">Saate eemaldada kõik töökontod (v. a mõjutatud konto), kasutades Windowsi sätteid > **juurdepääs tööle või koolile**.</span><span class="sxs-lookup"><span data-stu-id="97c9c-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="97c9c-105">[Tühjendage Office ' i mandaat](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows mandaadi halduri abil.</span><span class="sxs-lookup"><span data-stu-id="97c9c-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="97c9c-106">**Märkus:** Office 2016 registrite teed on muudetud versiooniks 16,0.</span><span class="sxs-lookup"><span data-stu-id="97c9c-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="97c9c-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="97c9c-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="97c9c-108">Avage Office ' i rakendus, **Valige**  >  **konto**  >  **Logi välja**. Seejärel logige sisse kasutaja kontoga, kellel on kehtiv litsents.</span><span class="sxs-lookup"><span data-stu-id="97c9c-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="97c9c-109">Lisateavet vt teemast [Office’i kontod](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="97c9c-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="97c9c-110">Maci kasutajad võiksid lugeda artiklit [Office 2016 for Maci rakendusse ei saa sisse logida](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="97c9c-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="97c9c-111">Lisateavet leiate teemast ["Kahjuks on teie ettevõtte teine konto juba selles arvutis sisse logitud" Office ' is](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span><span class="sxs-lookup"><span data-stu-id="97c9c-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>