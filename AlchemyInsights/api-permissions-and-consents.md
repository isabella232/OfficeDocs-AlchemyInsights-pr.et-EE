---
title: API load ja nõusolek
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974373"
---
# <a name="api-permissions-and-consent"></a><span data-ttu-id="8d304-102">API load ja nõusolek</span><span class="sxs-lookup"><span data-stu-id="8d304-102">API permissions and consent</span></span>

<span data-ttu-id="8d304-103">Microsoft Identity platformiga integreeritud rakendused järgivad loa mudelit, mis annab kasutajatele ja administraatoritele ülevaate sellest, kuidas andmeid saab kasutada.</span><span class="sxs-lookup"><span data-stu-id="8d304-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="8d304-104">Loa mudeli rakendamine on Microsofti identiteedi platvormi lõpp-punktis uuendatud.</span><span class="sxs-lookup"><span data-stu-id="8d304-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="8d304-105">See muudab viisi, kuidas rakendus peab Microsoft Identity platformiga suhtlema.</span><span class="sxs-lookup"><span data-stu-id="8d304-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="8d304-106">[Microsofti identiteedi platvormi lõpp-punktides olevad load ja nõusolek](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) hõlmavad selle loa mudeli põhimõisteid (sh ulatused, load ja nõusolek).</span><span class="sxs-lookup"><span data-stu-id="8d304-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="8d304-107">[Azure Active Directory (AZURE ad) nõusoleku raamistiku](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) abil on lihtne arendada mitme rentniku veebirakendust ja kohalikku klientrakendust.</span><span class="sxs-lookup"><span data-stu-id="8d304-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="8d304-108">Need rakendused lubavad sisse logida kasutaja kontodelt Azure AD rentniku jaoks, mis erineb rakenduse registreerimisest.</span><span class="sxs-lookup"><span data-stu-id="8d304-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="8d304-109">Lisaks on võimalik, et lisaks oma veebirakendusliidestele on neil vaja juurde pääseda ka veebi API-de (nt Microsoft Graph API) (Microsoft 365 Azure AD, Intune ' i ja teenuste jaoks) ning muude Microsofti teenuste API-de jaoks.</span><span class="sxs-lookup"><span data-stu-id="8d304-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>

