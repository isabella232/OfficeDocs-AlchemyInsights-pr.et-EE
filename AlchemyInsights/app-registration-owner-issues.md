---
title: Rakenduse registreerimise omaniku probleemid
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404455"
---
# <a name="app-registration-owner-issues"></a><span data-ttu-id="92992-102">Rakenduse registreerimise omaniku probleemid</span><span class="sxs-lookup"><span data-stu-id="92992-102">App Registration Owner issues</span></span>

<span data-ttu-id="92992-103">Järgmised on saadaval meetodid subjektide lisamiseks rakenduse registreerimise omanikeks.</span><span class="sxs-lookup"><span data-stu-id="92992-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="92992-104">Azure AD PowerShelli mooduli kasutamine –</span><span class="sxs-lookup"><span data-stu-id="92992-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="92992-105">Viide: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="92992-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="92992-106">Azure'i CLI- `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="92992-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="92992-107">Viide: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="92992-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="92992-108">MS Graphi kasutamine</span><span class="sxs-lookup"><span data-stu-id="92992-108">Using MS Graph -</span></span>

    <span data-ttu-id="92992-109">Viide: [omaniku lisamine – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="92992-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="92992-110">Azure AD portaali kasutamine – liikuge [lehele portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Valige > Owners > Add Owners (Omanikud)</span><span class="sxs-lookup"><span data-stu-id="92992-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="92992-111">**Kas te ei saa rakenduse registreerimiste teral oma rakendust vaadata, kuigi olete selle rakenduse omanik?**</span><span class="sxs-lookup"><span data-stu-id="92992-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="92992-112">Rakenduse omanik pole haldusroll.</span><span class="sxs-lookup"><span data-stu-id="92992-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="92992-113">Kui säte [Piira juurdepääsu Azure AD haldusportaalile](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) on lubatud, saab ainult administraator rakendusi vaadata rakenduse registreerimise portaalis.</span><span class="sxs-lookup"><span data-stu-id="92992-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="92992-114">Kui soovite, et omanik saaks rakendusi vaadata, keelake see säte (Määra see NO-ks) või määrake omanikule administraatori roll ainult konkreetse rakenduse jaoks.</span><span class="sxs-lookup"><span data-stu-id="92992-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="92992-115">Selleks on aga vaja Azure AD Premium P2 litsentsi ja lubada [privilegeeritud identiteedihaldus.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)</span><span class="sxs-lookup"><span data-stu-id="92992-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>
