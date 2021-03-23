---
title: Azure AD liitunud seadmete ühekordse sisselogimise tõrkeotsing
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
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035467"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="792c0-102">Azure AD liitunud seadmete ühekordse sisselogimise tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="792c0-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="792c0-103">Kui teil on kohapealne Active Directory (AD) keskkond ja soovite liituda oma AD domeeniga liitunud arvutitega Azure AD-ga, saate selle saavutamiseks kasutada hübriid Azure AD Liitu.</span><span class="sxs-lookup"><span data-stu-id="792c0-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="792c0-104">[Kuidas: teie hübriid-Azure Active Directory liitumise kavandamine](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) annab teile sellega seotud juhised hübriid-Azure AD joini rakendamiseks teie keskkonnas.</span><span class="sxs-lookup"><span data-stu-id="792c0-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="792c0-105">Lisateavet leiate teemast [AZURE ad liitunud seadmete konfigureerimine kohapealsete Single-Sign jaoks Windows Hello for δri abil](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span><span class="sxs-lookup"><span data-stu-id="792c0-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="792c0-106">**Esmase värskendamise turbelubade (PRT) probleemid**</span><span class="sxs-lookup"><span data-stu-id="792c0-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="792c0-107">Esmane värskendussagedus (PRT) on Windows 10, Windows Server 2016 ja uuemates versioonides, iOS-i ja Androidi seadmetes Azure AD autentimise peamine artefakt.</span><span class="sxs-lookup"><span data-stu-id="792c0-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="792c0-108">See on JSON-veebimärk (JWT), mis on spetsiaalselt välja antud Microsoft First Party turbelubade vahendajatele, et lubada ühekordse sisselogimise (SSO) kasutamist nendes seadmetes kasutatavates rakendustes.</span><span class="sxs-lookup"><span data-stu-id="792c0-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="792c0-109">Lisateavet selle kohta, kuidas PRT on Windows 10 seadmetes välja antud, kasutatud ja kaitstud, leiate teemast [mis on esmane värskendatav märk?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="792c0-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="792c0-110">**WamDefaultSet: Jah ja AzureADPrt: Jah**</span><span class="sxs-lookup"><span data-stu-id="792c0-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="792c0-111">Need väljad näitavad, kas kasutaja on seadmesse sisselogimisel Azure AD-sse autentinud.</span><span class="sxs-lookup"><span data-stu-id="792c0-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="792c0-112">Kui väärtused on **ei**, võib selle põhjus olla järgmine.</span><span class="sxs-lookup"><span data-stu-id="792c0-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="792c0-113">Vigane salvestusseade, mis on seadmega seotud TPM-iga registreerimisel (Kontrollige KeySignTest töötamise ajal)</span><span class="sxs-lookup"><span data-stu-id="792c0-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="792c0-114">Alternatiivne sisselogimise ID</span><span class="sxs-lookup"><span data-stu-id="792c0-114">Alternate Login ID</span></span>
- <span data-ttu-id="792c0-115">HTTP puhverserverit ei leitud</span><span class="sxs-lookup"><span data-stu-id="792c0-115">HTTP Proxy not found</span></span>

<span data-ttu-id="792c0-116">Dsregcmd käsuga seadmete tõrkeotsingu kohta leiate teavet artiklist [SSO olek](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="792c0-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
