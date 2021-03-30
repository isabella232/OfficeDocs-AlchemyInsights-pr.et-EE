---
title: Rakenduse registreerimise kliendi salajase või serdiga seotud probleemid
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
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404458"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="f38d4-102">Rakenduse registreerimise kliendi salajase või serdiga seotud probleemid</span><span class="sxs-lookup"><span data-stu-id="f38d4-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="f38d4-103">Kas rakendusklient aegub salaja?</span><span class="sxs-lookup"><span data-stu-id="f38d4-103">Application client secret expiring?</span></span>

<span data-ttu-id="f38d4-104">Olenemata sellest, kuidas registreeritud rakendus loodi( kas rakenduste registreerimise portaalis tavapärase registreerimisprotsessi kaudu või kui teenusesubjekt loodi teie rentnikus rakenduse nõusoleku alusel), tuleb enne praeguse rakendusekoodi aegumist luua uus kliendisaladus.</span><span class="sxs-lookup"><span data-stu-id="f38d4-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="f38d4-105">Maksimaalne kehtivusaeg on 2 aastat.</span><span class="sxs-lookup"><span data-stu-id="f38d4-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="f38d4-106">Meeldetuletusena tuleb salajane väärtus salvestada, kuna see ei ole enam nähtav pärast portaalis rakenduse registreerimiste lehelt lahkumist.</span><span class="sxs-lookup"><span data-stu-id="f38d4-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="f38d4-107">Lisateavet leiate teemast [Quickstart: Rakenduse](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) registreerimine Microsofti identiteediplatvormil ja Microsofti [identiteediplatvormi head tavad.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)</span><span class="sxs-lookup"><span data-stu-id="f38d4-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="f38d4-108">Lisateavet leiate teemast [Azure AD-rakenduse & teenusesubjekti loomine portaalis – Microsofti identiteediplatvorm](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span><span class="sxs-lookup"><span data-stu-id="f38d4-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>
