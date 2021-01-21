---
title: Märkide eluea konfigureerimine ja laiendamine
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916823"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="642df-102">Märkide eluea konfigureerimine ja laiendamine</span><span class="sxs-lookup"><span data-stu-id="642df-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="642df-103">Saate määrata Microsoft Identity Platformi poolt välja antud Accessi, SAML või ID-tõendi kestuse.</span><span class="sxs-lookup"><span data-stu-id="642df-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="642df-104">Saate määrata märkide eluea kõigi oma asutuse rakenduste jaoks, mitme rentniku (mitme organisatsiooni) rakenduse jaoks või ettevõtte teatud teenuse põhiosa jaoks.</span><span class="sxs-lookup"><span data-stu-id="642df-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="642df-105">Lisateavet leiate teemast [Konfigureeritav sümboolne kasutusaeg](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="642df-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="642df-106">Näiteid leiate teemast [märkide eluea konfigureerimine](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="642df-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="642df-107">Lisateavet selle kohta, kuidas konfigureerida Azure Active Directory B2C (Azure AD B2C) loa kehtivust ja ühilduvust, leiate teemast [märkide konfigureerimine Azure Active DIRECTORY B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span><span class="sxs-lookup"><span data-stu-id="642df-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="642df-108">[Azure Active DIRECTORY B2C seansi käitumise konfigureerimine](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) selles artiklis kirjeldatakse AZURE ad B2C kasutatavaid ühekordse SISSELOGIMISE (SSO) meetodeid ja see aitab teil poliitika konfigureerimisel valida kõige sobivama SSO meetodi.</span><span class="sxs-lookup"><span data-stu-id="642df-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="642df-109">**Kui kaua märgid kestavad? Kui kaua need kehtivad?**</span><span class="sxs-lookup"><span data-stu-id="642df-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="642df-110">Märkide eluiga on 1 tund ja seansi kasutusaeg on 24 tundi.</span><span class="sxs-lookup"><span data-stu-id="642df-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="642df-111">See tähendab, et kui 24 tunni jooksul pole taotlusi esitatud, peate enne uue loa taotlemist uuesti sisse logima.</span><span class="sxs-lookup"><span data-stu-id="642df-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="642df-112">Pärast 30. mail 2020 ei saa uut rentnikku kasutada konfigureeritav sümboolne eluaegset poliitikat seansi ja märkide värskendamise konfigureerimiseks.</span><span class="sxs-lookup"><span data-stu-id="642df-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="642df-113">Aegumine juhtub mitme kuu jooksul pärast seda, mis tähendab, et me lõpetame olemasoleva seansi austamise ja märkide värskendamise.</span><span class="sxs-lookup"><span data-stu-id="642df-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="642df-114">Saate ikkagi konfigureerida juurdepääsu turbelubade eluea pärast selle möödumist.</span><span class="sxs-lookup"><span data-stu-id="642df-114">You can still configure access token lifetimes after the deprecation.</span></span>






