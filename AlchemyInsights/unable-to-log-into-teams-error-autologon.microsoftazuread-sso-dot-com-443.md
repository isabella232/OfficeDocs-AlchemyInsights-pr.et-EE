---
title: Tõrke autologon.microsoftazuread-sso.com:443 tõttu ei saa Teamsi sisse logida
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931902"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="ee9c8-102">Tõrke autologon.microsoftazuread-sso dot com:443 tõttu ei saa Teamsi sisse logida</span><span class="sxs-lookup"><span data-stu-id="ee9c8-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="ee9c8-103">Kui O365 autentimisena on lubatud sujuv SSO, võib sisevõrgu saitide jaoks olla vajalik lisada URL „autologon.microsoftazuread-sso.com“.</span><span class="sxs-lookup"><span data-stu-id="ee9c8-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="ee9c8-104">Kui see on eelnevalt lisatud usaldusväärsete saitide hulka ja kasutusel on sujuv SSO, tuleks see usaldusväärsete saitide seast eemaldada.</span><span class="sxs-lookup"><span data-stu-id="ee9c8-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="ee9c8-105">Vaadake teemat [Tõrgeteta SSO tõrkeotsingu kontroll-loend](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span><span class="sxs-lookup"><span data-stu-id="ee9c8-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="ee9c8-106">URL-i sisevõrgu saitide loendisse lisamieks järgige järgmisi samme.</span><span class="sxs-lookup"><span data-stu-id="ee9c8-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="ee9c8-107">Avage Internet Explorer, klõpsates nuppu **Start**.</span><span class="sxs-lookup"><span data-stu-id="ee9c8-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="ee9c8-108">Tippige otsinguväljale Internet Explorer ja seejärel klõpsake tulemite loendis valikut **Internet Explorer**.</span><span class="sxs-lookup"><span data-stu-id="ee9c8-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="ee9c8-109">Klõpsake nuppu **Tööriistad** ja seejärel klõpsake valikut **Interneti-suvandid**.</span><span class="sxs-lookup"><span data-stu-id="ee9c8-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="ee9c8-110">Klõpsake vahekaarti **Turvalisus**.</span><span class="sxs-lookup"><span data-stu-id="ee9c8-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="ee9c8-111">Nüüd klõpsake suvandit **Kohaliku sisevõrgu saidid** ja seejärel klõpsake **saitide** nuppu ja seejärel nuppu **Täpsemalt**.</span><span class="sxs-lookup"><span data-stu-id="ee9c8-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="ee9c8-112">Sisestage veebisaidi URL ja klõpsake suvandit **Lisa**.</span><span class="sxs-lookup"><span data-stu-id="ee9c8-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="ee9c8-113">Kui olete lõpetanud, klõpsake suvandit **Sulge**.</span><span class="sxs-lookup"><span data-stu-id="ee9c8-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="ee9c8-114">Lisateavet leiate teemast [O365 sujuva SSO juurutamise dokumentatsioon](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (sh poliitikal põhinev protsess, mis lisab 3. juhises sisevõrgu saitidele URL-i).</span><span class="sxs-lookup"><span data-stu-id="ee9c8-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
