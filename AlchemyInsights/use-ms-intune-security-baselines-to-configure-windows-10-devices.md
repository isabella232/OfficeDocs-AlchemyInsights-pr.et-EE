---
title: Windows 10 seadmete konfigureerimine Microsoft Intune Security bases abil
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573401"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="2e2c9-102">Windows 10 seadmete konfigureerimine Microsoft Intune Security bases abil</span><span class="sxs-lookup"><span data-stu-id="2e2c9-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="2e2c9-103">Turvalisuse alused aitavad kaitsta kasutajaid ja seadmeid.</span><span class="sxs-lookup"><span data-stu-id="2e2c9-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="2e2c9-104">Turvalisuse alused on Windowsi sätted ' eelkonfigureeritud rühmad, mida kasutatakse teadaolevate rühma sätete ja vastavate turbe-rühmade soovitatud vaikeväärtuste rakendamiseks.</span><span class="sxs-lookup"><span data-stu-id="2e2c9-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="2e2c9-105">Kui loote Intune ' i turbe põhiprofiili, saate luua malli, mis koosneb mitmest seadme konfiguratsiooni profiilist.</span><span class="sxs-lookup"><span data-stu-id="2e2c9-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="2e2c9-106">Kui juurutate turvalisuse tasemeid kasutajate või seadmete rühmades, rakendatakse sätteid Windows 10 või uuema versiooniga töötavate seadmete jaoks.</span><span class="sxs-lookup"><span data-stu-id="2e2c9-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="2e2c9-107">Näiteks MDM Security Base automaatselt (1) lubab BitLocker for eemaldatavad draivid, (2) nõuab seadme lukustamise parooli ja (3) keelab põhiautentimise.</span><span class="sxs-lookup"><span data-stu-id="2e2c9-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="2e2c9-108">Kui vaikeväärtus ei tööta teie keskkonna jaoks, kohandage võrdlusalust, et rakendada vajalikke sätteid.</span><span class="sxs-lookup"><span data-stu-id="2e2c9-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="2e2c9-109">Turvalisuse põhialused aitavad luua ka lõpuga turvalise töövoo Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2e2c9-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="2e2c9-110">Järgmised eelised on järgmised.</span><span class="sxs-lookup"><span data-stu-id="2e2c9-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="2e2c9-111">Turvalisuse põhialus sisaldab turvalisust mõjutavatele sätetele häid tavasid ja soovitusi.</span><span class="sxs-lookup"><span data-stu-id="2e2c9-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="2e2c9-112">Kuna Intune ' i partnerid Windowsi turvalisuse meeskonnaga, mis loob rühmapoliitika jaoks baseid, põhinevad need soovitused kindlatel juhistel ja laialdastel kogemustel.</span><span class="sxs-lookup"><span data-stu-id="2e2c9-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="2e2c9-113">Kui teil on uus Intune ' is ja te pole kindel, kust alustada, siis turvalisuse alused aitavad teil kiiresti luua ja juurutada turvalist profiili.</span><span class="sxs-lookup"><span data-stu-id="2e2c9-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="2e2c9-114">Kui kasutate praegu rühmapoliitika, siis migreerimine Intune ' i juhtimiseks on palju hõlpsam, sest need on loodud Intune ' i ja hõlmavad ka juhtimise tipptaseme võimalusi.</span><span class="sxs-lookup"><span data-stu-id="2e2c9-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="2e2c9-115">Lisateavet leiate teemast [Windowsi turvalisuse alused](https://go.microsoft.com/fwlink/?linkid=2141503) ja [mobiilsideseadmete haldus](https://go.microsoft.com/fwlink/?linkid=2141701).</span><span class="sxs-lookup"><span data-stu-id="2e2c9-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>