---
title: IOS-seadmete Microsoft Intune ' is registreerimisega seotud probleemide tõrkeotsing
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708958"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="4dfc5-102">IOS-seadmete Microsoft Intune ' is registreerimisega seotud probleemide tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="4dfc5-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="4dfc5-103">Probleemi lahendamiseks vaadake allpool loetletud ressursid üle.</span><span class="sxs-lookup"><span data-stu-id="4dfc5-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="4dfc5-104">Levinumad tõrketeated ja eraldusvõime toimingud.</span><span class="sxs-lookup"><span data-stu-id="4dfc5-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="4dfc5-105">**Seadme kork on täis** Kasutajal on rohkem seadmeid, kui seadme limiit on registreeritud.</span><span class="sxs-lookup"><span data-stu-id="4dfc5-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="4dfc5-106">Vaadake need dokumendid üle, et [seade eemaldada](https://docs.microsoft.com/intune/devices-wipe) või [muuta seadme limiiti](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="4dfc5-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="4dfc5-107">**See teenus pole toetatud. Pole liitumise poliitikat:** Apple push Notification Service (APNS) peab olema konfigureeritud või uuendatud.</span><span class="sxs-lookup"><span data-stu-id="4dfc5-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="4dfc5-108">Lugege [selle dokumendi](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) juhiseid selle kohta, kuidas seda teha.</span><span class="sxs-lookup"><span data-stu-id="4dfc5-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="4dfc5-109">**Kasutaja litsentsi tüüp ei sobi või kasutajanime ei tuvastata:** Kasutajale tuleb määrata Intune või EMS-i litsents.</span><span class="sxs-lookup"><span data-stu-id="4dfc5-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="4dfc5-110">Vaadake need dokumendid üle, et määrata litsents: [Office halduskeskus](https://docs.microsoft.com/intune/licenses-assign) või Azure ' i [portaal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="4dfc5-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="4dfc5-111">Probleemi lahendamiseks täiendavad ressursid.</span><span class="sxs-lookup"><span data-stu-id="4dfc5-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="4dfc5-112">Saate kasutada [Intune tõrkeotsingu portaali](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) levinud liitumise tõrgete diagnoosimiseks ja lahendamiseks.</span><span class="sxs-lookup"><span data-stu-id="4dfc5-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="4dfc5-113">Lisateabe saamiseks vaadake [seda dokumenti](https://docs.microsoft.com/intune/help-desk-operators) üle.</span><span class="sxs-lookup"><span data-stu-id="4dfc5-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="4dfc5-114">Vaadake need dokumendid läbi nende levinud tõrgete loend, mis takistavad iga kasutaja registreerimist ja eraldusvõimet: [veaotsingu tõrkeotsing](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ja [tõrkeotsingu dokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="4dfc5-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="4dfc5-115">[Siit saate teada, kuidas Microsoft Intune ' is iOS-i seadmeid registreerida](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="4dfc5-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

