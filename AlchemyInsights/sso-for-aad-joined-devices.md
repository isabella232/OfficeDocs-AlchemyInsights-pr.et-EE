---
title: Single-Sign Active Directoryga ühendatud seadmete jaoks
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404591"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="5620f-102">Ühekordne sisselogimine Azure Active Directory liidetud seadmete jaoks</span><span class="sxs-lookup"><span data-stu-id="5620f-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="5620f-103">Kui teil on kohapealne Active Directory (AD) keskkond ja soovite liituda oma AD domeeniga ühendatud arvutitega Azure AD-ga, saate seda teha azure AD-hübriidjuurutuse abil.</span><span class="sxs-lookup"><span data-stu-id="5620f-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="5620f-104">[Juhised. Azure Active Directory hübriidjuurutuse plaanimine](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) pakub teile seotud juhiseid Azure AD hübriidjuurutuse juurutamiseks oma keskkonnas.</span><span class="sxs-lookup"><span data-stu-id="5620f-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="5620f-105">Azure AD-ga ühendatud seadmete konfigureerimine Single-Sign Windows Hello for Businessi abil</span><span class="sxs-lookup"><span data-stu-id="5620f-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="5620f-106">**Primaarse värskendamise loaga (PRT) seotud probleemid** Primaarne värskendustõend (PRT) on Windows 10, Windows Server 2016 ja uuemate versioonide, iOS-i ja Androidi seadmete Azure AD-autentimise põhiartist.</span><span class="sxs-lookup"><span data-stu-id="5620f-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="5620f-107">See on JSON Web Token (JWT), mis on spetsiaalselt välja antud Microsofti esimese osapoole loamaakleritele, et võimaldada ühekordset sisselogimist (SSO) kõigis nendes seadmetes kasutatavates rakendustes.</span><span class="sxs-lookup"><span data-stu-id="5620f-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="5620f-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)( Mis on esmane värskendustõend?) anname teada, kuidas PRT-d windows 10 seadmetes välja antakse, kasutatakse ja kaitstakse.</span><span class="sxs-lookup"><span data-stu-id="5620f-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="5620f-109">**WamDefaultSet: YES ja AzureADPrt: YES** Need väljad näitavad, kas kasutaja on seadmesse sisselogimisel Azure AD-ga autenditud.</span><span class="sxs-lookup"><span data-stu-id="5620f-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="5620f-110">Kui väärtused on **NO,** võib selle tähtaeg olla järgmine.</span><span class="sxs-lookup"><span data-stu-id="5620f-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="5620f-111">Seadmega registreerumisel seostatud TPM-i halb salvestusvõti (kontrollige administraatoriõigustes töötades klahvisignTesti).</span><span class="sxs-lookup"><span data-stu-id="5620f-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="5620f-112">Alternatiivne sisselogimistunnus</span><span class="sxs-lookup"><span data-stu-id="5620f-112">Alternate Login ID</span></span>
- <span data-ttu-id="5620f-113">HTTP-puhverserverit ei leitud</span><span class="sxs-lookup"><span data-stu-id="5620f-113">HTTP Proxy not found</span></span>

<span data-ttu-id="5620f-114">Seadmete tõrkeotsing käsu dsregcmd abil – [SSO olek](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="5620f-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
