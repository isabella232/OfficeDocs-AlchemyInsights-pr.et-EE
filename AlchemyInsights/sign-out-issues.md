---
title: Väljalogimisega seotud probleemid
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7793"
- "9004355"
ms.openlocfilehash: 794e5c43340ba4b5c653eda4c11b4480cd3fa710
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900867"
---
# <a name="sign-out-issues"></a><span data-ttu-id="94960-102">Väljalogimisega seotud probleemid</span><span class="sxs-lookup"><span data-stu-id="94960-102">Sign-out issues</span></span>

<span data-ttu-id="94960-103">Väljalogimisega seotud probleemide lahendamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="94960-103">To resolve issues related to signing out, perform the following steps:</span></span>

1. <span data-ttu-id="94960-104">Kui teie või kasutaja saab sisselogitud või väljavisatud rakendustest, järgige artiklite juhiseid, et [konfigureerida autentimise seansi haldus tingimusjuurdepääsu](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) või konfigureeritav [sümboolne eluiga Microsoft Identity Platform ' is](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="94960-104">If you or a user are getting logged or kicked out of applications, follow the guidance in the articles [Configure authentication session management with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) or [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>
2. <span data-ttu-id="94960-105">Enamik muid väljalogimise tõrkeid või probleeme saab lahendada, kui tõrkeotsing Azure Active Directory (Azure AD) integreerimisele konkreetse rakendusega.</span><span class="sxs-lookup"><span data-stu-id="94960-105">Most other sign-out errors or problems can be solved by troubleshooting the integration of Azure Active Directory (Azure AD) with the specific application.</span></span> <span data-ttu-id="94960-106">Mõne kindla integratsiooni kohta leiate juhised selle kohta, kuidas [Azure Active Directory rakenduste integreerimiseks seda kollektsiooni](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)kasutada, sealhulgas:</span><span class="sxs-lookup"><span data-stu-id="94960-106">You can find guidance for a specific integration by going to this [collection of tutorials for integrating applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list), including:</span></span>
    - <span data-ttu-id="94960-107">SaaS Application Tutorials</span><span class="sxs-lookup"><span data-stu-id="94960-107">SaaS application tutorials</span></span>
    - <span data-ttu-id="94960-108">Ühekordse sisselogimise õpetused</span><span class="sxs-lookup"><span data-stu-id="94960-108">Single sign-on tutorials</span></span>
    - <span data-ttu-id="94960-109">Kasutaja-ettevalmistamine Tutorials</span><span class="sxs-lookup"><span data-stu-id="94960-109">User-provisioning tutorials</span></span>