---
title: Microsoft Intune'is Windowsi seadmete registreerimisega seotud probleemide tõrkeotsing
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808967"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="6132b-102">Microsoft Intune'is Windowsi seadmete registreerimisega seotud probleemide tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="6132b-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="6132b-103">Vaadake allpool loetletud ressursid üle, et probleem kohe lahendada.</span><span class="sxs-lookup"><span data-stu-id="6132b-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="6132b-104">Levinumad tõrketeated ja eraldusvõime juhised.</span><span class="sxs-lookup"><span data-stu-id="6132b-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="6132b-105">**Tarkvara ei saa installida, 0x80cf4017.** Teie konto sert on aegunud.</span><span class="sxs-lookup"><span data-stu-id="6132b-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="6132b-106">Laadige PC-kliendi tarkvarapakett Intune'i halduskonsoolis uuesti alla.</span><span class="sxs-lookup"><span data-stu-id="6132b-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="6132b-107">Lisateabe saamiseks vaadake seda dokumentatsiooni.</span><span class="sxs-lookup"><span data-stu-id="6132b-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="6132b-108">**Tõrkekood 0x801c0003:** Tõrge võib ilmneda järgmistel juhtudel.</span><span class="sxs-lookup"><span data-stu-id="6132b-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="6132b-109">Kasutajal on rohkem seadmeid, mis on registreeritud kui seadme limiit.</span><span class="sxs-lookup"><span data-stu-id="6132b-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="6132b-110">Vaadake need dokumendid [üle, et eemaldada seade](https://docs.microsoft.com/intune/devices-wipe) [või muuta seadme piirangut.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="6132b-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="6132b-111">"Kasutajad võivad seadmetega Azure AD-ga liituda" on seatud väärtusele "pole".</span><span class="sxs-lookup"><span data-stu-id="6132b-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="6132b-112">Määrake see kõigile või valige kasutajad.</span><span class="sxs-lookup"><span data-stu-id="6132b-112">Set it to all or select users.</span></span> <span data-ttu-id="6132b-113">Lisateabe [saamiseks vaadake](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) seda dokumentatsiooni.</span><span class="sxs-lookup"><span data-stu-id="6132b-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="6132b-114">Teine kasutaja on seadme juba registreerinud.</span><span class="sxs-lookup"><span data-stu-id="6132b-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="6132b-115">Sel juhul eemaldage seade Azure Intune'i konsoolist või eemaldage seade enne uuesti proovimist käsitsi.</span><span class="sxs-lookup"><span data-stu-id="6132b-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="6132b-116">Seade on Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="6132b-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="6132b-117">Azure Active Directoryga saavad liituda ainult Windows 10 Pro, Education ja Enterprise SKUs.</span><span class="sxs-lookup"><span data-stu-id="6132b-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="6132b-118">Täiendavad ressursid probleemi lahendamiseks.</span><span class="sxs-lookup"><span data-stu-id="6132b-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="6132b-119">[Intune'i tõrkeotsinguportaali](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) abil saate diagnoosida ja lahendada levinumaid registreerimistõrkeid.</span><span class="sxs-lookup"><span data-stu-id="6132b-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="6132b-120">Lisateavet [leiate sellest](https://docs.microsoft.com/intune/help-desk-operators) dokumendist.</span><span class="sxs-lookup"><span data-stu-id="6132b-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="6132b-121">Vaadake need dokumendid üle, et saada ülevaade levinumatest vigadest, mis takistavad registreerimist ja lahendamist: tõrkeotsingu [juhend ja](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) [tõrkeotsingu dokument.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="6132b-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="6132b-122">[Saate teada, kuidas registreerida Windowsi seadmeid Microsoft Intune'is.](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="6132b-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
