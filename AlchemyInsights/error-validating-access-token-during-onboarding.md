---
title: Ilmnes tõrge juurdepääsuloa tõrke valideerimisel töölaua analüüs-pardalemineku ajal
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741160"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="6cad6-102">"Ilmnes tõrge valideerimisel juurdepääsu luba" tõrge töölaua analüüs kasutuselevõtt</span><span class="sxs-lookup"><span data-stu-id="6cad6-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="6cad6-103">See tõrge täheldatakse tavaliselt autentimise luba aegub.</span><span class="sxs-lookup"><span data-stu-id="6cad6-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="6cad6-104">Tavaliselt värskendab lehe värskendamine luba.</span><span class="sxs-lookup"><span data-stu-id="6cad6-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="6cad6-105">Kuid see probleem võib püsida, kui on olemas tingimuslik juurdepääsupoliitika rakendatud konto on kasutusel pardal Desktop Analytics.</span><span class="sxs-lookup"><span data-stu-id="6cad6-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="6cad6-106">Saate vaadata Azure AD Logi sisse logid Azure ' i portaalis, et näha, kas on mis tahes sisselogimise tõrked konto kasutatakse töölaua analüüs kasutuselevõtt.</span><span class="sxs-lookup"><span data-stu-id="6cad6-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="6cad6-107">Tingimusliku juurdepääsu kohta lisateabe saamiseks külastage [oma tingimusjuurdepääsu juurutamine](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="6cad6-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>