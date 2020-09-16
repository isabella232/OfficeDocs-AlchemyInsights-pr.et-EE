---
title: Intune poliitikate ja profiilide loomine
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1064"
- "6700005"
ms.openlocfilehash: 9026beac824ebc3849241dbb534c27b00ef1d0eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47746755"
---
# <a name="creating-intune-policy-and-profiles"></a><span data-ttu-id="53579-102">Intune poliitika ja profiilide loomine</span><span class="sxs-lookup"><span data-stu-id="53579-102">Creating Intune policy and profiles</span></span>

<span data-ttu-id="53579-103">Intune ' is saate luua erinevaid asju sisaldavaid poliitikaid ja profiile.</span><span class="sxs-lookup"><span data-stu-id="53579-103">In Intune, you can create policies and profiles that do different things.</span></span>

- <span data-ttu-id="53579-104">**Registreerimise profiilid**: seadmete konfigureerimine platvormi järgi, kasutajate afiinsuse lubamine, mitme teguri autentimine ja palju muud.</span><span class="sxs-lookup"><span data-stu-id="53579-104">**Enrollment profiles**: Preconfigure your devices by platform, enable user affinity, use multi-factor authentication, and more.</span></span>

  <span data-ttu-id="53579-105">[See, mis on seadme registreerimine](https://docs.microsoft.com/intune/device-enrollment), ja luua rakendustes [Androidi](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll)-i, [macOS](https://docs.microsoft.com/intune/macos-enroll)-i ja [Windowsiga](https://docs.microsoft.com/intune/windows-enrollment-methods) liitumise profiilid on head ressursid.</span><span class="sxs-lookup"><span data-stu-id="53579-105">[What is device enrollment](https://docs.microsoft.com/intune/device-enrollment), and create enrollment profiles for [Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll), and [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) are good resources.</span></span>

- <span data-ttu-id="53579-106">**Nõuetele vastavuse poliitika**: Määratlege reeglid ja sätted, mida seadmed peavad järgima, et need vastaksid nõuetele.</span><span class="sxs-lookup"><span data-stu-id="53579-106">**Compliance policies**: Define the rules and settings that devices must follow to be compliant.</span></span> <span data-ttu-id="53579-107">Samuti saate kasutada seadmete jälgimiseks vastavuskontrolli põhimõtteid ning teavitada kasutajaid mittevastavusest.</span><span class="sxs-lookup"><span data-stu-id="53579-107">You can also use compliance policies to monitor devices, and notify users of non-compliance.</span></span>

  <span data-ttu-id="53579-108">[Seadme nõuetele vastavuse poliitikate](https://docs.microsoft.com/intune/device-compliance-get-started)kasutamise alustamine.</span><span class="sxs-lookup"><span data-stu-id="53579-108">Get started with [device compliance policies](https://docs.microsoft.com/intune/device-compliance-get-started).</span></span>
- <span data-ttu-id="53579-109">**Tingimusliku juurdepääsu poliitikad**: aitavad tagada organisatsiooni ressursside, olenevalt teie sisestatud tingimustest.</span><span class="sxs-lookup"><span data-stu-id="53579-109">**Conditional access policies**: Help secure organizational resources, depending on conditions that you enter.</span></span> <span data-ttu-id="53579-110">Kui teil on näiteks seadmed, mis pole ühilduvad, kasutage juurdepääsu piiramiseks meilile ja SharePointi juurdepääsule tingimusjuurdepääsu.</span><span class="sxs-lookup"><span data-stu-id="53579-110">For example, for devices that aren't compliant, use conditional access to restrict access to email and SharePoint.</span></span>

  <span data-ttu-id="53579-111">[Mis on tingimusjuurdepääsu](https://docs.microsoft.com/intune/conditional-access) ja [levinud moodused tingimusjuurdepääsu kasutamiseks](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) , on alustamiseks head ressursid.</span><span class="sxs-lookup"><span data-stu-id="53579-111">[What is conditional access](https://docs.microsoft.com/intune/conditional-access) and [common ways to use conditional access](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) are good resources to get started.</span></span>

- <span data-ttu-id="53579-112">**Konfiguratsiooni profiilid**: funktsioonide ja sätete haldamine seadmetes (sh meilisätted), WiFi-võrgu lisamine, sisseehitatud mallide kasutamine, iOS-i ja macOS-i seadme funktsioonide haldamine ning palju muud.</span><span class="sxs-lookup"><span data-stu-id="53579-112">**Configuration profiles**: Manage features and settings on devices, including email settings, add a WiFi network, use built-in templates, control iOS and macOS device features, and more.</span></span>

  <span data-ttu-id="53579-113">[Seadme konfigureerimise profiilidega](https://docs.microsoft.com/intune/device-profiles)alustamine.</span><span class="sxs-lookup"><span data-stu-id="53579-113">Get started at [device configuration profiles](https://docs.microsoft.com/intune/device-profiles).</span></span>

<span data-ttu-id="53579-114">Kasulikud lingid:</span><span class="sxs-lookup"><span data-stu-id="53579-114">Helpful links:</span></span>

- [<span data-ttu-id="53579-115">Levinumad küsimused, probleemid ja resolutsioonid seadme poliitikate ja profiilidega Intune ' is</span><span class="sxs-lookup"><span data-stu-id="53579-115">Common questions, issues, and resolutions with device policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/device-profile-troubleshoot)

- [<span data-ttu-id="53579-116">Poliitikate ja profiilide tõrkeotsing Intune ' is</span><span class="sxs-lookup"><span data-stu-id="53579-116">Troubleshoot policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
