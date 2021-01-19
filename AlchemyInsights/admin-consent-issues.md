---
title: Administraatori nõusoleku probleemid
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900930"
---
# <a name="admin-consent-issues"></a><span data-ttu-id="15b27-102">Administraatori nõusoleku probleemid</span><span class="sxs-lookup"><span data-stu-id="15b27-102">Admin consent issues</span></span>

1. <span data-ttu-id="15b27-103">Lubage administraatori [nõusoleku töövoog](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) , et lubada kasutajatel taotleda administraatori kinnitust otse nõusoleku kuvalt.</span><span class="sxs-lookup"><span data-stu-id="15b27-103">Enable the [admin consent workflow](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) to allow users to request administrator approval directly from the consent screen.</span></span>

1. <span data-ttu-id="15b27-104">Kui teie või teie rakenduse kasutajad näevad nõusoleku käigus ette ootamatuid tõrkeid, lugege seda artiklit tõrkeotsingu toimingute tegemiseks: [ootamatu tõrge rakenduse nõusoleku](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)andmisel.</span><span class="sxs-lookup"><span data-stu-id="15b27-104">If you or your application's users are seeing unexpected errors during the consent process, see this article for troubleshooting steps: [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>

1. <span data-ttu-id="15b27-105">Lugege lisateavet [Microsofti identiteedi platvormi administraatori nõusoleku kohta](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)ja selle kohta, kuidas [nõusolekut küsimine](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) toimib ning kuidas [hinnata rentniku kogu administraatori nõusoleku taotlust](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span><span class="sxs-lookup"><span data-stu-id="15b27-105">Learn more about [Admin consent on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), how the [consent prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) works, and how to [evaluate a request for tenant-wide admin consent](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span></span>

1. <span data-ttu-id="15b27-106">Microsoft Identity platformiga integreeritud rakendused järgivad loa mudelit, mis annab kasutajatele ja administraatoritele ülevaate sellest, kuidas andmeid saab kasutada.</span><span class="sxs-lookup"><span data-stu-id="15b27-106">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="15b27-107">Loa mudeli rakendamine on värskendatud Microsofti identiteedi platvormi lõpp-punkti ja see muudab seda, kuidas rakendus peab Microsoft Identity platformiga suhtlema.</span><span class="sxs-lookup"><span data-stu-id="15b27-107">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint, and it changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="15b27-108">Selle loa mudeli (sh ulatuse, õiguse ja nõusoleku) ülevaate saamiseks lugege [Microsofti identiteedi platvormi lõpp-punkti "permissions" ja "nõusolek"](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) .</span><span class="sxs-lookup"><span data-stu-id="15b27-108">See [Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for an overview of this authorization model, including scopes, permissions, and consent.</span></span>