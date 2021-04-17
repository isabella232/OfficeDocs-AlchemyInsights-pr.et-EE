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
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833071"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="db9cf-102">Microsoft 365 rakenduste parandamine sõnum "Kahjuks on teie asutuse teine konto juba sisse logitud".</span><span class="sxs-lookup"><span data-stu-id="db9cf-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="db9cf-103">Probleemi lahendamiseks proovige järgmist.</span><span class="sxs-lookup"><span data-stu-id="db9cf-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="db9cf-104">Eemaldage kõik töökontod (v.a mõjutatud konto), kasutades Windowsi > **Accessi töö- või koolisätteid.**</span><span class="sxs-lookup"><span data-stu-id="db9cf-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="db9cf-105">[Tühjendage Windowsi identimisteabe](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) halduri abil Office'i identimisteavet.</span><span class="sxs-lookup"><span data-stu-id="db9cf-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="db9cf-106">**Märkus.** Office 2016 registriteed on muutunud 16.0-ks.</span><span class="sxs-lookup"><span data-stu-id="db9cf-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="db9cf-107">(Nt: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="db9cf-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="db9cf-108">Avage Office'i rakendus ja valige **Fail**  >  **Konto**  >  **logi välja**. Seejärel logige sisse kehtiva litsentsiga kasutajakontoga.</span><span class="sxs-lookup"><span data-stu-id="db9cf-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="db9cf-109">Lisateavet vt teemast [Office’i kontod](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="db9cf-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="db9cf-110">Maci kasutajad võiksid lugeda artiklit [Office 2016 for Maci rakendusse ei saa sisse logida](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="db9cf-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="db9cf-111">Lisateavet leiate Office'is teemast "Kahjuks on teie ettevõtte teine konto selles arvutis juba sisse [logitud".](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)</span><span class="sxs-lookup"><span data-stu-id="db9cf-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>