---
title: Tõrkeotsingu kasutamine Windowsi seadmetes Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8c5e7cc502d016ad658383685523dc240dfb4dc6
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29661521"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="74303-102">Tõrkeotsingu kasutamine Windowsi seadmetes Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="74303-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="74303-103">Läbi nende lahendamiseks nüüd allpool loetletud ressurssidele.</span><span class="sxs-lookup"><span data-stu-id="74303-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="74303-104">Mõned levinud tõrketeated ja lahendus:</span><span class="sxs-lookup"><span data-stu-id="74303-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="74303-p101">**Ei saa installida tarkvara, 0x80cf4017:** Teie konto sert on aegunud. Uuesti laadida PC kliendi tarkvara paketi Intune konsoolis. Läbi selle dokumentatsioonist.</span><span class="sxs-lookup"><span data-stu-id="74303-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="74303-108">**Tõrkekood 0x801c0003:** Tõrge võib ilmneda järgmistel juhtudel:</span><span class="sxs-lookup"><span data-stu-id="74303-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="74303-p102">Kasutajal on rohkem kui seadme seadmete. Läbi nende dokumentide [seade eemaldada](https://docs.microsoft.com/intune/devices-wipe) või [muuta seadme piirang](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="74303-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="74303-p103">"Kasutajad võivad ühendada seadmeid Azure AD" on seatud "ei ole". Määrata kõigile või kasutajad. Vaadake lisateabe saamiseks [selle dokumentatsiooni](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .</span><span class="sxs-lookup"><span data-stu-id="74303-p103">"Users may join devices to Azure AD" is set to "none". Set it to all or select users. Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="74303-p104">Mõni teine kasutaja on juba registreeritud seadme. Kui see juhtub, Eemalda seadme Azure Intune konsooli või käsitsi unenroll seade enne uuesti proovimist.</span><span class="sxs-lookup"><span data-stu-id="74303-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="74303-p105">Seade on Windows 10 Home. Ainult Windows 10 Pro, hariduse ja ettevõtluse SKUs saab liituda Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="74303-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="74303-118">Lisaressursse, mis probleemi lahendada:</span><span class="sxs-lookup"><span data-stu-id="74303-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="74303-p106">Diagnoosimiseks ja lahendamiseks ühise registreerimise rikete [Intune tõrkeotsingu portaali](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) abil. Läbi [selle dokumendi](https://docs.microsoft.com/intune/help-desk-operators) lisateabe saamiseks.</span><span class="sxs-lookup"><span data-stu-id="74303-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="74303-121">Läbi nende dokumentide nimekiri kõige sagedasemad vead, mis takistavad registreerimine ja lahendused igale: [tõrkeotsing juhend](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ja [tõrkeotsing doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="74303-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="74303-122">[Kuidas registreeruda Windowsi seadmetes Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="74303-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
  

