---
title: Kasutaja nõusoleku tõrkeotsing
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
- "9004353"
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901187"
---
# <a name="troubleshoot-user-consent"></a><span data-ttu-id="52413-102">Kasutaja nõusoleku tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="52413-102">Troubleshoot user consent</span></span>

1. <span data-ttu-id="52413-103">Saate konfigureerida, kuidas lõppkasutajad Azure ' i portaali või PowerShelli kaudu rakendustega nõustuvad.</span><span class="sxs-lookup"><span data-stu-id="52413-103">You can configure how end-users consent to applications through the Azure Portal or PowerShell.</span></span> <span data-ttu-id="52413-104">Lisateavet leiate teemast [kasutaja nõusoleku sätted](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) .</span><span class="sxs-lookup"><span data-stu-id="52413-104">See [User consent settings](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for more information.</span></span>
1. <span data-ttu-id="52413-105">Administraator saab kasutada ka [Microsoft GRAPHI API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) -d ühe kasutaja nimel delegeeritud õigustele nõusoleku andmiseks.</span><span class="sxs-lookup"><span data-stu-id="52413-105">An administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="52413-106">Lisateavet leiate teemast [juurdepääsu saamine kasutaja nimel](https://docs.microsoft.com/graph/auth-v2-user).</span><span class="sxs-lookup"><span data-stu-id="52413-106">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>
1. <span data-ttu-id="52413-107">[Kasutaja nõusoleku tõrked](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): selles artiklis käsitletakse tõrkeid, mis võivad ilmneda rakenduse jaoks nõusoleku andmise protsessi käigus.</span><span class="sxs-lookup"><span data-stu-id="52413-107">[User Consent Errors](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): this article discusses errors that can occur during the process of consenting to an application.</span></span> <span data-ttu-id="52413-108">Kui teil on probleeme ootamatu nõusoleku küsimisega, mis ei sisalda tõrketeateid, lugege teemat [AZURE ad ' i autentimise stsenaariumid](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="52413-108">If you are troubleshooting unexpected consent prompts that do not contain any error messages, see [Authentication Scenarios for Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>