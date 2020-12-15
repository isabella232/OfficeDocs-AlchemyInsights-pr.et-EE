---
title: Microsoft Intune ' i kasutamine veebipääsu haldamiseks rakenduses Microsoft Edge iOS-i ja Androidi jaoks
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
ms.openlocfilehash: 4d6ab4df4ff9588ce5052421602e347c76c91c3f
ms.sourcegitcommit: a7952283882d341515623d5ae58eda14d0553449
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/10/2020
ms.locfileid: "49677447"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="e363b-102">Microsoft Intune ' i kasutamine veebipääsu haldamiseks rakenduses Microsoft Edge iOS-i ja Androidi jaoks</span><span class="sxs-lookup"><span data-stu-id="e363b-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="e363b-103">Microsoft Edge iOS-i ja Androidi jaoks võimaldab kasutajal sirvida veebi mitmest täiesti eraldiseisvast profiilist.</span><span class="sxs-lookup"><span data-stu-id="e363b-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="e363b-104">Microsoft 365 andmete laiem kaitse on saadaval siis, kui tellite Enterprise Mobility + Security Suite ' i, mis sisaldab Microsoft Intune ' i ja Azure Active Directory Premiumi funktsioone (nt tingimusjuurdepääsu).</span><span class="sxs-lookup"><span data-stu-id="e363b-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="e363b-105">Vähemalt soovite juurutada tingimusjuurdepääsu poliitika, mis (1) võimaldab kasutajatel iOS-i ja Androidi kaudu Microsoft Edge ' i mobiilsideseadmete kaudu ühendust võtta ja et (2) rakendab Microsoft Intune ' i rakenduse kaitsepoliitika, mis tagab kaitstud sirvimise kogemuse.</span><span class="sxs-lookup"><span data-stu-id="e363b-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="e363b-106">Lisateavet tingimusjuurdepääsu ja-poliitikate kasutamise kohta leiate järgmistest teemadest.</span><span class="sxs-lookup"><span data-stu-id="e363b-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="e363b-107">Azure Active Directory rakendamine tingimusjuurdepääsu poliitikate rakendamiseks</span><span class="sxs-lookup"><span data-stu-id="e363b-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="e363b-108">Microsoft Intune ' i rakenduse kaitsmise poliitikate loomine</span><span class="sxs-lookup"><span data-stu-id="e363b-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="e363b-109">Ühekordse sisselogimise kasutamine Azure Active Directory jaoks – ühendatud veebirakendused poliitikaga kaitstud brauserites</span><span class="sxs-lookup"><span data-stu-id="e363b-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="e363b-110">Rakenduse konfiguratsiooni kasutamine sirvimise kogemuse haldamiseks</span><span class="sxs-lookup"><span data-stu-id="e363b-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="e363b-111">Ainult töö-ja koolide kontode kasutamise lubamine</span><span class="sxs-lookup"><span data-stu-id="e363b-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="e363b-112">Rakenduse üldist konfigureerimine poliitikate juurutamine</span><span class="sxs-lookup"><span data-stu-id="e363b-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="e363b-113">Rakenduse konfigureerimise poliitikate juurutamine andmete kaitsmiseks</span><span class="sxs-lookup"><span data-stu-id="e363b-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="e363b-114">Microsoft Endpoint Manageri kasutamine rakenduse konfigureerimise poliitikate juurutamiseks</span><span class="sxs-lookup"><span data-stu-id="e363b-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="e363b-115">Hallatavate rakenduste logidele juurdepääsemise kohta leiate teavet teemast [Microsoft Edge ' i kasutamine iOS-i ja Androidi jaoks](https://go.microsoft.com/fwlink/?linkid=2132578).</span><span class="sxs-lookup"><span data-stu-id="e363b-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
