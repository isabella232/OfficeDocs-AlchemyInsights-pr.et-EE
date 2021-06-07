---
title: Turbejoonte Microsoft Intune kasutamine Windows 10 seadmetes
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793699"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="68df8-102">Turbejoonte Microsoft Intune kasutamine Windows 10 seadmetes</span><span class="sxs-lookup"><span data-stu-id="68df8-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="68df8-103">Intune'i turbealused aitavad kaitsta kasutajaid ja seadmeid.</span><span class="sxs-lookup"><span data-stu-id="68df8-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="68df8-104">Turbealused on Windows sätete eel konfigureeritud rühmad, mida kasutatakse vastavate turberühmade soovitatud teadaolevate sätete ja vaikeväärtuste rühma rakendamiseks.</span><span class="sxs-lookup"><span data-stu-id="68df8-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="68df8-105">Intune'i turbe alusprofiili loomisega loote malli, mis koosneb mitmest seadme konfiguratsiooniprofiilist.</span><span class="sxs-lookup"><span data-stu-id="68df8-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="68df8-106">Kui juurutate turbealused kasutajate või seadmete rühmadele, rakendatakse sätted seadmetele, mis käitavad Windows 10 uuemates versioonides.</span><span class="sxs-lookup"><span data-stu-id="68df8-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="68df8-107">Näiteks Microsofti mobiilsideseadmete halduse (MDM) turbealus lubab BitLocker irdkettatele, nõuab seadme vabastamiseks parooli ja keelab elementaarse autentimise.</span><span class="sxs-lookup"><span data-stu-id="68df8-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="68df8-108">Kui teie keskkonnas vaikeväärtus ei tööta, saate kohandada lähtejoont, et rakendada nõudeid, mida vajate.</span><span class="sxs-lookup"><span data-stu-id="68df8-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="68df8-109">Turbealused aitavad luua ka Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="68df8-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="68df8-110">Turbealus sisaldab turbega seotud sätete parimaid tavasid ja soovitusi.</span><span class="sxs-lookup"><span data-stu-id="68df8-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="68df8-111">Intune'i partnerid Windows turbemeeskonnaga, kes loob rühmapoliitikate jaoks alusjooned, seega põhinevad need soovitused tugevatel juhistel ja ulatuslikul kogemusel.</span><span class="sxs-lookup"><span data-stu-id="68df8-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="68df8-112">Kui olete Intune'i uus kasutaja ja pole kindel, kust alustada, aitavad turbealused kiiresti luua ja juurutada turvalise profiili.</span><span class="sxs-lookup"><span data-stu-id="68df8-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="68df8-113">Kui kasutate praegu rühmapoliitikat, on migreerimine Intune'i haldamise eesmärgil palju lihtsam turbealustega, kuna need on intune'i sisse ehitatud ja sisaldavad tipptasemel haldusfunktsioone.</span><span class="sxs-lookup"><span data-stu-id="68df8-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="68df8-114">Lisateavet leiate teemast Windows [turbealused ja](/windows/security/threat-protection/windows-security-baselines) [Mobiilsideseadmete haldus.](/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="68df8-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

