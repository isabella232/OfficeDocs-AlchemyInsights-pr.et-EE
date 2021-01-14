---
title: Tõrgeteta SSO integreerimise probleemid kohapealsete rakendustega
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868675"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a><span data-ttu-id="b3589-102">Tõrgeteta SSO integreerimise probleemid kohapealsete rakendustega</span><span class="sxs-lookup"><span data-stu-id="b3589-102">Issues with integrating Seamless SSO with my on-premises apps</span></span>

<span data-ttu-id="b3589-103">Tõrgeteta SSO integreerimise probleemide lahendamiseks kohapealsete rakendustega tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="b3589-103">To troubleshoot issues with integrating Seamless SSO with on-premises applications, do the following:</span></span>

<span data-ttu-id="b3589-104">**Soovitatavad toimingud**</span><span class="sxs-lookup"><span data-stu-id="b3589-104">**Recommended steps**</span></span>

1. <span data-ttu-id="b3589-105">**Kohapealse rakenduse** konfigureerimiseks **ühekordse sisselogimise rakenduse puhverserveri kaudu** leiate teavet teemast [paroolide häälestamine ühekordse sisselogimise jaoks rakenduse puhverserveriga](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span><span class="sxs-lookup"><span data-stu-id="b3589-105">To configure an **on-premises application** for **single sign-on through Application Proxy**, see [Password vaulting for single sign-on with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span></span>
1. <span data-ttu-id="b3589-106">**Rakenduse puhverserveri probleemide tõrkeotsing**: Soovitame alustada läbivaatust tõrkeotsingu voo, [siluda rakenduse puhverserveri konnektori probleeme](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), et kindlaks teha, kas rakenduse puhverserveri konnektorid on õigesti konfigureeritud.</span><span class="sxs-lookup"><span data-stu-id="b3589-106">**Troubleshooting Application Proxy issues**: we recommend that you start with reviewing the troubleshooting flow, [Debug Application Proxy Connector issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), to determine if Application Proxy connectors are configured correctly.</span></span> <span data-ttu-id="b3589-107">Kui teil on endiselt probleeme rakendusega ühenduse loomisega, järgige tõrkeotsingu juhiseid rakenduses [debug rakenduse puhverserveri probleemid](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span><span class="sxs-lookup"><span data-stu-id="b3589-107">If you're still having trouble connecting to the application, follow the troubleshooting steps in [Debug Application Proxy application issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span></span> <span data-ttu-id="b3589-108">[Cors probleemide tuvastamiseks](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) saate kasutada järgmisi brauseri debug tööriistu.</span><span class="sxs-lookup"><span data-stu-id="b3589-108">You can [identify CORS issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) by using the following browser debug tools:</span></span>
    1. <span data-ttu-id="b3589-109">Käivitage brauser ja liikuge sirvides veebi rakendusse.</span><span class="sxs-lookup"><span data-stu-id="b3589-109">Launch the browser and browse to the web app.</span></span>
    1. <span data-ttu-id="b3589-110">Debug konsooli kuvamiseks vajutage klahvi **F12** .</span><span class="sxs-lookup"><span data-stu-id="b3589-110">Press **F12** to bring up the debug console.</span></span>
    1. <span data-ttu-id="b3589-111">Proovi reprodutseerida tehing ja vaadata konsooli sõnum.</span><span class="sxs-lookup"><span data-stu-id="b3589-111">Try to reproduce the transaction, and review the console message.</span></span> <span data-ttu-id="b3589-112">CORS rikkumine tekitab konsooli tõrke päritolu kohta.</span><span class="sxs-lookup"><span data-stu-id="b3589-112">A CORS violation produces a console error about origin.</span></span>
    1. <span data-ttu-id="b3589-113">Mõnda CORS probleemi ei saa lahendada (nt kui teie rakendus suunab autentimiseks login.microsoftonline.com ja juurdepääsuluba aegub).</span><span class="sxs-lookup"><span data-stu-id="b3589-113">Some CORS issues can't be resolved, such as when your app redirects to login.microsoftonline.com to authenticate, and the access token expires.</span></span> <span data-ttu-id="b3589-114">CORS kõne nurjub.</span><span class="sxs-lookup"><span data-stu-id="b3589-114">The CORS call then fails.</span></span> <span data-ttu-id="b3589-115">Selle stsenaariumi lahendus on pikendada juurdepääsuluba, et takistada selle kehtivust kasutaja seansi ajal.</span><span class="sxs-lookup"><span data-stu-id="b3589-115">A workaround for this scenario is to extend the lifetime of the access token, to prevent it from expiring during a user’s session.</span></span> <span data-ttu-id="b3589-116">Lisateavet selle kohta leiate teemast [Konfigureeritav turbelubade eluiga Microsoft Identity Platform ' is](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="b3589-116">For more information about how to do this, see [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="b3589-117">**Soovitatavad dokumendid**</span><span class="sxs-lookup"><span data-stu-id="b3589-117">**Recommended documents**</span></span>

- [<span data-ttu-id="b3589-118">Ühekordse sisselogimise konfigureerimine rakenduse puhverserveri rakendusse</span><span class="sxs-lookup"><span data-stu-id="b3589-118">How to configure single sign-on to an Application Proxy application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [<span data-ttu-id="b3589-119">SAML ühekordse sisselogimise rakendused rakenduse puhverserveriga</span><span class="sxs-lookup"><span data-stu-id="b3589-119">SAML single sign-on for on-premises applications with Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [<span data-ttu-id="b3589-120">Azure Active Directory rakenduse puhverserveri CORS probleemide mõistmine ja lahendamine</span><span class="sxs-lookup"><span data-stu-id="b3589-120">Understand and solve Azure Active Directory Application Proxy CORS issues</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [<span data-ttu-id="b3589-121">Kerberose piiratud delegeerimise konfiguratsioonide tõrkeotsing rakenduse puhverserveri korral</span><span class="sxs-lookup"><span data-stu-id="b3589-121">Troubleshoot Kerberos constrained delegation configurations for Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)