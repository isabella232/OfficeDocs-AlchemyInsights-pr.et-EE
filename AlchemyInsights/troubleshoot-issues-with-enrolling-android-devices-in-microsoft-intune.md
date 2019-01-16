---
title: Tõrkeotsingu kasutamine Microsoft Intune Android seadmete
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 2f4fc434128ebe7323f0b8c08aec3be82112bbda
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28286220"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="cb871-102">Tõrkeotsingu kasutamine Microsoft Intune Android seadmete</span><span class="sxs-lookup"><span data-stu-id="cb871-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="cb871-103">Läbi nende lahendamiseks nüüd allpool loetletud ressurssidele.</span><span class="sxs-lookup"><span data-stu-id="cb871-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="cb871-104">Mõned levinud probleemid ja lahendus:</span><span class="sxs-lookup"><span data-stu-id="cb871-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="cb871-p101">**Seadme krüptimata Ettevõtjaportaal viga:** Android, eriti alates v7.0, uuemad versioonid nõuavad pääsukoodi käivitamisel veenduge, et seade on täielikult krüptitud. Käivituse PIN-koodi või täielikult seadme krüptimine on ühiseid lahendusi. Läbi [selle dokumendi](https://docs.microsoft.com/en-us/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) lisateabe.</span><span class="sxs-lookup"><span data-stu-id="cb871-p101">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted. Common solutions are to enable a startup pin or fully encrypt the device. Review [this document](https://docs.microsoft.com/en-us/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span> 
  
 <span data-ttu-id="cb871-p102">**Seadmed ei saate Intune service sisse või kuvada Intune konsoolis "Unhealthy":** Mõned Samsung 4.4 ja 5,5 seadmed võivad kontrolli teenindusse. Seal on 3 võimalikud lahendused selle probleemi:</span><span class="sxs-lookup"><span data-stu-id="cb871-p102">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service. There are 3 possible solutions to this issue:</span></span> 
  
1. <span data-ttu-id="cb871-110">Käsitsi avada Intune Ettevõtjaportaal app, mis algatab automaatselt seadme sünkroonimine.</span><span class="sxs-lookup"><span data-stu-id="cb871-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>
    
2. <span data-ttu-id="cb871-111">Värskendage seadme Android 6.0 või kõrgem.</span><span class="sxs-lookup"><span data-stu-id="cb871-111">Update the device to Android 6.0 or higher.</span></span>
    
3. <span data-ttu-id="cb871-p103">Keelata Samsung Smart Manager hallata Intune'i Ettevõtjaportaal. Läbi [selle dokumendi](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) täpsemat teavet need probleemid ja lahendused.</span><span class="sxs-lookup"><span data-stu-id="cb871-p103">Disable Samsung Smart Manager from managing the Intune Company Portal. Review [this document](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span> 
    
 <span data-ttu-id="cb871-p104">**Kasutaja litsentsi tüüp ei sobi** või **kasutaja nimi tundmatu tõrge:** kasutaja peab olema määratud Intune või EMS litsentsi. Läbi nende dokumentide kaudu litsentsi omistamiseks: Office administreerimiskeskuse või Azure portaali.</span><span class="sxs-lookup"><span data-stu-id="cb871-p104">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span> 
  
<span data-ttu-id="cb871-116">Lisaressursse, mis probleemi lahendada:</span><span class="sxs-lookup"><span data-stu-id="cb871-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="cb871-p105">Diagnoosimiseks ja lahendamiseks ühise registreerimise rikete [Intune tõrkeotsingu portaali](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) abil. Läbi [selle dokumendi](https://docs.microsoft.com/en-us/intune/help-desk-operators) lisateabe saamiseks.</span><span class="sxs-lookup"><span data-stu-id="cb871-p105">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="cb871-119">Nimekiri kõige sagedasemad vead, mis takistavad registreerimine ja lahendused igale [dokumendi](https://docs.microsoft.com/en-us/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) läbivaatamiseks.</span><span class="sxs-lookup"><span data-stu-id="cb871-119">Review [this document](https://docs.microsoft.com/en-us/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span> 
    
3. <span data-ttu-id="cb871-120">[Kuidas registreeruda Microsoft Intune Androidiga](https://docs.microsoft.com/en-us/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="cb871-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/android-enroll).</span></span>
    

