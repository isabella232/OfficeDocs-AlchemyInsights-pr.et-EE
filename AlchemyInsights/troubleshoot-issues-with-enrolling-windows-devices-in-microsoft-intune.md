---
title: Microsofti Intune ' i Windowsi seadmetega seotud probleemide tõrkeotsing
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665828"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="26dc8-102">Microsofti Intune ' i Windowsi seadmetega seotud probleemide tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="26dc8-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="26dc8-103">Vaadake allpool loetletud ressursid probleemi lahendamiseks kohe.</span><span class="sxs-lookup"><span data-stu-id="26dc8-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="26dc8-104">Mõned levinud tõrketeated ja eraldusvõime sammud:</span><span class="sxs-lookup"><span data-stu-id="26dc8-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="26dc8-105">**Tarkvara ei saa installida, 0x80cf4017:** Teie kontosert on aegunud.</span><span class="sxs-lookup"><span data-stu-id="26dc8-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="26dc8-106">Uuesti alla laadida arvuti kliendi tarkvarapakett Intune konsoolis.</span><span class="sxs-lookup"><span data-stu-id="26dc8-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="26dc8-107">Lisateabe saamiseks vaadake seda dokumentatsiooni.</span><span class="sxs-lookup"><span data-stu-id="26dc8-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="26dc8-108">**Tõrkekood 0x801c0003:** Tõrge võib ilmneda järgmistel juhtudel:</span><span class="sxs-lookup"><span data-stu-id="26dc8-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="26dc8-109">Kasutajal on rohkem seadmeid, mis on registreeritud kui seadme piirang.</span><span class="sxs-lookup"><span data-stu-id="26dc8-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="26dc8-110">Vaadake neid dokumente [seadme eemaldamiseks](https://docs.microsoft.com/intune/devices-wipe) või [seadme piirangu muutmiseks](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="26dc8-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="26dc8-111">"Kasutajad võivad liituda seadmete Azure AD" on seatud "none."</span><span class="sxs-lookup"><span data-stu-id="26dc8-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="26dc8-112">Seadke see kõigile või valige kasutajad.</span><span class="sxs-lookup"><span data-stu-id="26dc8-112">Set it to all or select users.</span></span> <span data-ttu-id="26dc8-113">Lisateabe saamiseks vaadake [seda dokumentatsiooni](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .</span><span class="sxs-lookup"><span data-stu-id="26dc8-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="26dc8-114">Seade on juba teise kasutaja poolt registreeritud.</span><span class="sxs-lookup"><span data-stu-id="26dc8-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="26dc8-115">Kui see on nii, eemaldage seade Azure Intune konsooli või enne uuesti proovimist seadme käsitsi lahti.</span><span class="sxs-lookup"><span data-stu-id="26dc8-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="26dc8-116">Seade on Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="26dc8-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="26dc8-117">Azure Active Directoryga saab liituda ainult Windows 10 Pro, haridus ja Enterprise SKUs.</span><span class="sxs-lookup"><span data-stu-id="26dc8-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="26dc8-118">Täiendavad ressursid probleemi lahendamiseks:</span><span class="sxs-lookup"><span data-stu-id="26dc8-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="26dc8-119">Levinud registreerimise tõrgete diagnoosimiseks ja lahendamiseks kasutage [tõrkeotsingu portaali Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) .</span><span class="sxs-lookup"><span data-stu-id="26dc8-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="26dc8-120">Vaadake [seda dokumenti](https://docs.microsoft.com/intune/help-desk-operators) rohkem üksikasju.</span><span class="sxs-lookup"><span data-stu-id="26dc8-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="26dc8-121">Vaadake need dokumendid läbi levinud tõrgete loendi, mis takistavad registreerimise ja resolutsioonide iga: [tõrkeotsingu juhend](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ja [tõrkeotsingu doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="26dc8-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="26dc8-122">[Vaadake, kuidas Windowsi seadmeid Microsoft Intune ' is registreeruda](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="26dc8-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
