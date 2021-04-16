---
title: Töölauaanalüütika (Desktop Analytics) pardaleminemise ajal ilmnes juurdepääsulubade tõrke valideerimisel tõrge
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
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813684"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="63660-102">Töölauaanalüüsi kasutamise ajal ilmnes tõrge juurdepääsulubade valideerimisel</span><span class="sxs-lookup"><span data-stu-id="63660-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="63660-103">Seda tõrget järgitakse tavaliselt siis, kui autentimistõend aegub.</span><span class="sxs-lookup"><span data-stu-id="63660-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="63660-104">Tavaliselt värskendab lehe värskendamine luba.</span><span class="sxs-lookup"><span data-stu-id="63660-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="63660-105">See probleem võib siiski laheneda, kui kontole on rakendatud mõni tingimusjuurdepääsu poliitika, mida kasutatakse töölauaanalüüsis.</span><span class="sxs-lookup"><span data-stu-id="63660-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="63660-106">Azure AD sisselogimislogid saate azure'i portaalis läbi vaadata, et näha, kas töölauaanalüüsis kasutatava konto sisselogimisel ilmneb sisselogimistõrkeid.</span><span class="sxs-lookup"><span data-stu-id="63660-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="63660-107">Tingimusjuurutuse kohta leiate lisateavet teemast [Tingimusjuurutuse kavandamine.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)</span><span class="sxs-lookup"><span data-stu-id="63660-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>