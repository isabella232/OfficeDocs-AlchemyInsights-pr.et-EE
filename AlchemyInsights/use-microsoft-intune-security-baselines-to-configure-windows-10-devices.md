---
title: Windows 10 seadmete konfigureerimine Microsoft Intune Security bases abil
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50694436"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="80de3-102">Microsoft Intune ' i turvalisuse alused Windows 10 seadmete konfigureerimiseks</span><span class="sxs-lookup"><span data-stu-id="80de3-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="80de3-103">Turvalisuse alused aitavad kaitsta kasutajaid ja seadmeid.</span><span class="sxs-lookup"><span data-stu-id="80de3-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="80de3-104">Turvalisuse alused on Windowsi sätted ' eelkonfigureeritud rühmad, mida kasutatakse teadaolevate rühma sätete ja vastavate turbe-rühmade soovitatud vaikeväärtuste rakendamiseks.</span><span class="sxs-lookup"><span data-stu-id="80de3-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="80de3-105">Kui loote Intune ' i turbe põhiprofiili, saate luua malli, mis koosneb mitmest seadme konfiguratsiooni profiilist.</span><span class="sxs-lookup"><span data-stu-id="80de3-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="80de3-106">Kui juurutate turvalisuse tasemeid kasutajate või seadmete rühmades, rakendatakse sätteid Windows 10 või uuemates versioonides töötavate seadmete suhtes.</span><span class="sxs-lookup"><span data-stu-id="80de3-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="80de3-107">Näiteks Microsoft Mobile Device Management (MDM) Security Base automaatselt (1) lubab BitLocker for eemaldatavad draivid, (2) nõuab seadme lukustamise parooli ja (3) keelab põhiautentimise.</span><span class="sxs-lookup"><span data-stu-id="80de3-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="80de3-108">Kui vaikeväärtus ei tööta teie keskkonna jaoks, saate kohandada algseid sätteid, et rakendada vajalikke sätteid.</span><span class="sxs-lookup"><span data-stu-id="80de3-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="80de3-109">Turvalisuse põhialused aitavad luua ka lõpuga turvalise töövoo Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="80de3-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="80de3-110">Selle funktsiooni eelised on järgmised.</span><span class="sxs-lookup"><span data-stu-id="80de3-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="80de3-111">Turvalisuse põhialus sisaldab turvalisust mõjutavatele sätetele häid tavasid ja soovitusi.</span><span class="sxs-lookup"><span data-stu-id="80de3-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="80de3-112">Kuna Intune ' i partnerid Windowsi turvalisuse meeskonnaga, mis loob rühmapoliitika jaoks baseid, põhinevad need soovitused kindlatel juhistel ja laialdastel kogemustel.</span><span class="sxs-lookup"><span data-stu-id="80de3-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="80de3-113">Kui teil on uus Intune ' is ja te pole kindel, kust alustada, siis turvalisuse alused aitavad teil kiiresti luua ja juurutada turvalist profiili.</span><span class="sxs-lookup"><span data-stu-id="80de3-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="80de3-114">Kui kasutate praegu rühmapoliitika, siis migreerimine Intune ' i juhtimiseks on palju hõlpsam kui turvalisuse alused, sest need turvalisuse alused on loodud Intune ' i ja hõlmavad juhtimise tipptaseme võimalusi.</span><span class="sxs-lookup"><span data-stu-id="80de3-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="80de3-115">Lisateavet leiate teemast [Windowsi turvalisuse alused](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) ja [mobiilsideseadmete haldus](https://docs.microsoft.com/windows/client-management/mdm/).</span><span class="sxs-lookup"><span data-stu-id="80de3-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>