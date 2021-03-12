---
title: Paroolil põhinevate tõrgeteta ühekordse sisselogimise (SSO) probleemide tõrkeotsing
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
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714767"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="2dfc2-102">Paroolil põhinevate tõrgeteta ühekordse sisselogimise (SSO) probleemide tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="2dfc2-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="2dfc2-103">Parooli põhise SSO põhialuste kohta leiate teavet teemast [paroolide autentimine Azure Active Directory abil](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span><span class="sxs-lookup"><span data-stu-id="2dfc2-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="2dfc2-104">**Parooli põhise SSO konfigureerimine**</span><span class="sxs-lookup"><span data-stu-id="2dfc2-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="2dfc2-105">[Parooli põhise ühekordse sisselogimise konfigureerimine](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) – selles artiklis kirjeldatakse üksikasjalikumalt parooli põhise SSO suvandit.</span><span class="sxs-lookup"><span data-stu-id="2dfc2-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="2dfc2-106">Kui lisatav rakendus vajab kohandatud konfiguratsiooni ja te peate kasutama parooli põhiset SSO-d, siis see artikkel on teie jaoks.</span><span class="sxs-lookup"><span data-stu-id="2dfc2-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="2dfc2-107">[Parooli põhise ühekordse sisselogimise konfigureerimine – Prem rakendused](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) – rakenduse puhverserver toetab mitmeid ühekordse sisselogimise režiime.</span><span class="sxs-lookup"><span data-stu-id="2dfc2-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="2dfc2-108">Paroolil põhinev sisselogimine on mõeldud rakendustele, mis kasutavad autentimiseks kasutajanime/parooli kombinatsiooni.</span><span class="sxs-lookup"><span data-stu-id="2dfc2-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="2dfc2-109">Kui konfigureerite oma rakenduse jaoks parooli-põhise sisselogimise, peavad kasutajad olema sisse logitud kohapealsesse rakendusse.</span><span class="sxs-lookup"><span data-stu-id="2dfc2-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="2dfc2-110">Pärast seda salvestab Azure Active Directory sisselogimise teabe ja annab selle automaatselt rakendusele, kui kasutajad pääsevad sellele eemalt.</span><span class="sxs-lookup"><span data-stu-id="2dfc2-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="2dfc2-111">Sa peaksid juba avaldanud ja katsetanud oma rakendust rakenduse puhverserveriga.</span><span class="sxs-lookup"><span data-stu-id="2dfc2-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="2dfc2-112">Kui ei, siis järgige rakenduse [Avalda rakendusi AZURE ad Application proxy abil](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) , seejärel jätkake oma parooli baasil kasutatava SSO häälestamist ka Prem-rakenduste jaoks.</span><span class="sxs-lookup"><span data-stu-id="2dfc2-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="2dfc2-113">Parooli põhise SSO tõrkeotsingu kohta leiate teavet teemast [parooli põhine ühekordne sisselogimise tõrkeotsing AZURE ad](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="2dfc2-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>
