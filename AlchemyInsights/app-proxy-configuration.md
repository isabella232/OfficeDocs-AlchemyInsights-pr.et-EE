---
title: Rakenduse puhverserveri konfigureerimine
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885137"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="4da62-102">Rakenduse puhverserveri konfigureerimine</span><span class="sxs-lookup"><span data-stu-id="4da62-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="4da62-103">Kui soovite teada saada, kuidas konfigureerida rakenduse puhverserveri rakendust Azure AD-s asutusesisesete rakenduste pilve jaoks, lugege teemat [rakenduse puhverserveri rakenduse konfigureerimine](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span><span class="sxs-lookup"><span data-stu-id="4da62-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="4da62-104">Ühekordne sisselogimine (SSO) võimaldab kasutajatel kasutada rakendust, autentimata mitu korda.</span><span class="sxs-lookup"><span data-stu-id="4da62-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="4da62-105">See lubab ühes autentimisel esineda pilves, Azure Active Directory vastu ning lubab teenusel või konnektori kasutajal jäljendada kasutajat, kes täidavad rakenduse jaoks täiendavaid autentimise probleeme.</span><span class="sxs-lookup"><span data-stu-id="4da62-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="4da62-106">Lisateavet leiate teemast [ühekordse sisselogimise konfigureerimine rakenduse puhverserveri rakendusse](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span><span class="sxs-lookup"><span data-stu-id="4da62-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="4da62-107">Kasutage [seda artiklit](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) levinud probleemide tõrkeotsinguks, kui loote uue rakenduse puhverserveri rakenduse.</span><span class="sxs-lookup"><span data-stu-id="4da62-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="4da62-108">Kui teil on probleeme rakenduse back-end autentimise häälestamisega, peate võib-olla lahendama [Kerberose piiratud delegeerimise konfiguratsioonid rakenduse puhverserveri jaoks](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) või järgima juhiseid [rakenduse konfigureerimise kohta PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) abil probleemi lahendamiseks.</span><span class="sxs-lookup"><span data-stu-id="4da62-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>
