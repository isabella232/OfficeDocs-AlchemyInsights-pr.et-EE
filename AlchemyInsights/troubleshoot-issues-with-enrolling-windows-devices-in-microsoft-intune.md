---
title: Tõrkeotsingu kasutamine Windowsi seadmetes Microsoft Intune
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
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665828"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="5b546-102">Tõrkeotsingu kasutamine Windowsi seadmetes Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="5b546-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="5b546-103">Läbi nende lahendamiseks nüüd allpool loetletud ressurssidele.</span><span class="sxs-lookup"><span data-stu-id="5b546-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="5b546-104">Mõned levinud tõrketeated ja lahendus:</span><span class="sxs-lookup"><span data-stu-id="5b546-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="5b546-105">**Ei saa installida tarkvara, 0x80cf4017:** Teie konto sert on aegunud.</span><span class="sxs-lookup"><span data-stu-id="5b546-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="5b546-106">Uuesti laadida PC kliendi tarkvara paketi Intune konsoolis.</span><span class="sxs-lookup"><span data-stu-id="5b546-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="5b546-107">Läbi selle dokumentatsioonist.</span><span class="sxs-lookup"><span data-stu-id="5b546-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="5b546-108">**Tõrkekood 0x801c0003:** Tõrge võib ilmneda järgmistel juhtudel:</span><span class="sxs-lookup"><span data-stu-id="5b546-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="5b546-109">Kasutajal on rohkem kui seadme seadmete.</span><span class="sxs-lookup"><span data-stu-id="5b546-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="5b546-110">Läbi nende dokumentide [seade eemaldada](https://docs.microsoft.com/intune/devices-wipe) või [muuta seadme piirang](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="5b546-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="5b546-111">"Kasutajad võivad ühendada seadmeid Azure AD" on seatud "ei ole."</span><span class="sxs-lookup"><span data-stu-id="5b546-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="5b546-112">Määrata kõigile või kasutajad.</span><span class="sxs-lookup"><span data-stu-id="5b546-112">Set it to all or select users.</span></span> <span data-ttu-id="5b546-113">Vaadake lisateabe saamiseks [selle dokumentatsiooni](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .</span><span class="sxs-lookup"><span data-stu-id="5b546-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="5b546-114">Mõni teine kasutaja on juba registreeritud seadme.</span><span class="sxs-lookup"><span data-stu-id="5b546-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="5b546-115">Kui see juhtub, Eemalda seadme Azure Intune konsooli või käsitsi unenroll seade enne uuesti proovimist.</span><span class="sxs-lookup"><span data-stu-id="5b546-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="5b546-116">Seade on Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="5b546-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="5b546-117">Ainult Windows 10 Pro, hariduse ja ettevõtluse SKUs saab liituda Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5b546-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="5b546-118">Lisaressursse, mis probleemi lahendada:</span><span class="sxs-lookup"><span data-stu-id="5b546-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="5b546-119">Diagnoosimiseks ja lahendamiseks ühise registreerimise rikete [Intune tõrkeotsingu portaali](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) abil.</span><span class="sxs-lookup"><span data-stu-id="5b546-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="5b546-120">Läbi [selle dokumendi](https://docs.microsoft.com/intune/help-desk-operators) lisateabe saamiseks.</span><span class="sxs-lookup"><span data-stu-id="5b546-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="5b546-121">Läbi nende dokumentide nimekiri kõige sagedasemad vead, mis takistavad registreerimine ja lahendused igale: [tõrkeotsing juhend](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ja [tõrkeotsing doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="5b546-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="5b546-122">[Kuidas registreeruda Windowsi seadmetes Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="5b546-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
