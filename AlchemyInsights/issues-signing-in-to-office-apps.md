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
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579933"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="8397c-102">Microsoft 365 rakenduste parandamine "Vabandust, teine konto teie organisatsioonis on juba allkirjastatud" sõnum</span><span class="sxs-lookup"><span data-stu-id="8397c-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="8397c-103">Probleemi lahendamiseks proovige järgmist.</span><span class="sxs-lookup"><span data-stu-id="8397c-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="8397c-104">Eemaldage kõik töökontod, välja arvatud mõjutatud konto, kasutades Windowsi sätteid > **juurdepääsu töö või kooli**.</span><span class="sxs-lookup"><span data-stu-id="8397c-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="8397c-105">[Tühjendage Office ' i mandaat](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) , kasutades Windowsi mandaat Manager.</span><span class="sxs-lookup"><span data-stu-id="8397c-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="8397c-106">**Märkus:** Office 2016 registri teed on muutunud 16,0.</span><span class="sxs-lookup"><span data-stu-id="8397c-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="8397c-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="8397c-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="8397c-108">Avage Office ' i rakendus, valige **faili**  >  **konto**  >  **Logi välja**. Seejärel logige sisse, kasutades kehtivat litsentsi kasutajakontoga.</span><span class="sxs-lookup"><span data-stu-id="8397c-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="8397c-109">Lisateavet vt teemast [Office’i kontod](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="8397c-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="8397c-110">Maci kasutajad võiksid lugeda artiklit [Office 2016 for Maci rakendusse ei saa sisse logida](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="8397c-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="8397c-111">Lisateabe saamiseks vaadake ["Vabandust, teine konto teie organisatsioonis on juba sisse logitud selles arvutis" Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span><span class="sxs-lookup"><span data-stu-id="8397c-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>