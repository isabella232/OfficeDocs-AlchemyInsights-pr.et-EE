---
title: Windowsi seadmete registreerimisega seotud probleemide tõrkeotsing Microsoft Intune ' is
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658874"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="14e08-102">Windowsi seadmete registreerimisega seotud probleemide tõrkeotsing Microsoft Intune ' is</span><span class="sxs-lookup"><span data-stu-id="14e08-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="14e08-103">Probleemi lahendamiseks vaadake allpool loetletud ressursid üle.</span><span class="sxs-lookup"><span data-stu-id="14e08-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="14e08-104">Levinumad tõrketeated ja eraldusvõime toimingud.</span><span class="sxs-lookup"><span data-stu-id="14e08-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="14e08-105">**Tarkvara ei saa installida, 0x80cf4017.** Teie konto sert on aegunud.</span><span class="sxs-lookup"><span data-stu-id="14e08-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="14e08-106">Laadige PC-kliendi tarkvarapakett uuesti alla Intune konsoolis.</span><span class="sxs-lookup"><span data-stu-id="14e08-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="14e08-107">Lisateabe saamiseks vaadake seda dokumentatsiooni.</span><span class="sxs-lookup"><span data-stu-id="14e08-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="14e08-108">**Tõrkekood 0x801c0003:** Tõrge võib ilmneda järgmistel juhtudel.</span><span class="sxs-lookup"><span data-stu-id="14e08-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="14e08-109">Kasutajal on rohkem seadmeid, kui seadme limiit on registreeritud.</span><span class="sxs-lookup"><span data-stu-id="14e08-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="14e08-110">Vaadake need dokumendid üle, et [seade eemaldada](https://docs.microsoft.com/intune/devices-wipe) või [muuta seadme limiiti](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="14e08-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="14e08-111">"Kasutajad võivad ühendada seadmed Azure AD" on seatud "pole".</span><span class="sxs-lookup"><span data-stu-id="14e08-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="14e08-112">Määrake see kõigile või valige kasutajad.</span><span class="sxs-lookup"><span data-stu-id="14e08-112">Set it to all or select users.</span></span> <span data-ttu-id="14e08-113">Lisateabe saamiseks vaadake [seda dokumentatsiooni](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .</span><span class="sxs-lookup"><span data-stu-id="14e08-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="14e08-114">Teine kasutaja on seadme juba registreerinud.</span><span class="sxs-lookup"><span data-stu-id="14e08-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="14e08-115">Kui see on nii, eemaldage seade Azure ' i Intune ' i konsoolist või registreerige seade enne uuesti proovimist käsitsi.</span><span class="sxs-lookup"><span data-stu-id="14e08-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="14e08-116">Seade on Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="14e08-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="14e08-117">Azure Active Directoryga saab liituda ainult Windows 10 Pro, haridusasutuste ja Enterprise ' i SKUs.</span><span class="sxs-lookup"><span data-stu-id="14e08-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="14e08-118">Probleemi lahendamiseks täiendavad ressursid.</span><span class="sxs-lookup"><span data-stu-id="14e08-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="14e08-119">Saate kasutada [Intune tõrkeotsingu portaali](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) levinud liitumise tõrgete diagnoosimiseks ja lahendamiseks.</span><span class="sxs-lookup"><span data-stu-id="14e08-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="14e08-120">Lisateabe saamiseks vaadake [seda dokumenti](https://docs.microsoft.com/intune/help-desk-operators) üle.</span><span class="sxs-lookup"><span data-stu-id="14e08-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="14e08-121">Vaadake need dokumendid läbi nende levinud tõrgete loend, mis takistavad iga kasutaja registreerimist ja eraldusvõimet: [veaotsingu tõrkeotsing](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ja [tõrkeotsingu dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="14e08-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="14e08-122">[Siit saate teada, kuidas Windowsi seadmeid Microsoft Intune ' is registreerida](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="14e08-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
