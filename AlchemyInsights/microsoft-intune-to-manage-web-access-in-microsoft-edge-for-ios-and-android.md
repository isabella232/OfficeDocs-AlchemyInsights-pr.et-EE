---
title: Microsoft Intune'i kasutamine iOS-i ja Androidi jaoks mõeldud Microsoft Edge'i veebipääsu haldamiseks
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
- "9003846"
- "6895"
- "9006502"
- "11144"
ms.openlocfilehash: a6c6f9563933b7cf6b71c4758c29ffd94617c4be
ms.sourcegitcommit: 7a406a3d4680662e81f0056454f7e25fb2f52504
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/17/2021
ms.locfileid: "52989661"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="236fe-102">Microsoft Intune'i kasutamine iOS-i ja Androidi jaoks mõeldud Microsoft Edge'i veebipääsu haldamiseks</span><span class="sxs-lookup"><span data-stu-id="236fe-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="236fe-103">Microsoft Edge iOS-i ja Androidi jaoks võimaldab kasutajal veebi sirvida mitmest täiesti eraldi profiilist.</span><span class="sxs-lookup"><span data-stu-id="236fe-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="236fe-104">Microsoft 365 andmete kõige laiemad kaitsevõimalused muutuvad kättesaadavaks, kui tellite Enterprise Mobility + Security komplekti, mis sisaldab Microsoft Intune'i ja Azure Active Directory Premiumi funktsioone (nt tingimusjuurdepääsu).</span><span class="sxs-lookup"><span data-stu-id="236fe-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="236fe-105">Vähemalt soovite juurutada tingimusjuurdepääsu poliitika, mis (1) võimaldab kasutajatel luua ühenduse mobiilsideseadmetest Microsoft Edge'i iOS-i ja Androidi jaoks ning (2) rakendab Microsoft Intune'i rakendusekaitsepoliitika, mis pakub kaitstud sirvimiskogemust.</span><span class="sxs-lookup"><span data-stu-id="236fe-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="236fe-106">Tingimusjuurdepääsu ja poliitikate kasutamise kohta leiate teavet teemast</span><span class="sxs-lookup"><span data-stu-id="236fe-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="236fe-107">Azure Active Directory tingimusjuurdepääsu poliitikate rakendamist</span><span class="sxs-lookup"><span data-stu-id="236fe-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="236fe-108">Microsoft Intune'i rakenduse kaitsepoliitikate loomine</span><span class="sxs-lookup"><span data-stu-id="236fe-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="236fe-109">Ühekordse sisselogimise kasutamine Azure Active Directoryga ühendatud veebirakenduste jaoks poliitikaga kaitstud brauserites</span><span class="sxs-lookup"><span data-stu-id="236fe-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="236fe-110">Rakenduse konfiguratsiooni kasutamine sirvimiskogemuse haldamiseks</span><span class="sxs-lookup"><span data-stu-id="236fe-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="236fe-111">Luba kasutada ainult töö- ja koolikontosid</span><span class="sxs-lookup"><span data-stu-id="236fe-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="236fe-112">Rakenduse üldiste konfiguratsioonipoliitikate juurutamine</span><span class="sxs-lookup"><span data-stu-id="236fe-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="236fe-113">Rakenduse konfiguratsioonipoliitikate juurutamine andmekaitse jaoks</span><span class="sxs-lookup"><span data-stu-id="236fe-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="236fe-114">Rakenduse konfiguratsioonipoliitikate juurutamine Microsoft Endpoint Manageri abil</span><span class="sxs-lookup"><span data-stu-id="236fe-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="236fe-115">Teavet hallatud rakenduselogidele juurdepääsu kohta leiate teemast [Microsoft Edge'i kasutamine iOS-i ja Androidi jaoks hallatavatele rakenduselogidele juurdepääsemiseks.](https://go.microsoft.com/fwlink/?linkid=2132578)</span><span class="sxs-lookup"><span data-stu-id="236fe-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
