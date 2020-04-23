---
title: Microsoft Intune ' i sisseveeretavate iOS-i seadmetega seotud probleemide tõrkeotsing
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736154"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="8ad84-102">Microsoft Intune ' i sisseveeretavate iOS-i seadmetega seotud probleemide tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="8ad84-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="8ad84-103">Vaadake allpool loetletud ressursid probleemi lahendamiseks kohe.</span><span class="sxs-lookup"><span data-stu-id="8ad84-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="8ad84-104">Mõned levinud tõrketeated ja eraldusvõime sammud:</span><span class="sxs-lookup"><span data-stu-id="8ad84-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="8ad84-105">**Seadme kork on saavutatud** Kasutajal on rohkem seadmeid, mis on registreeritud kui seadme piirang.</span><span class="sxs-lookup"><span data-stu-id="8ad84-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="8ad84-106">Vaadake neid dokumente [seadme eemaldamiseks](https://docs.microsoft.com/intune/devices-wipe) või [seadme piirangu muutmiseks](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="8ad84-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="8ad84-107">**Seda teenust ei toetata. Ei ole registreerimine poliitika:** Apple push Notification Service (APNS) tuleb konfigureerida või uuendada.</span><span class="sxs-lookup"><span data-stu-id="8ad84-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="8ad84-108">Vaadake [seda dokumenti](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) juhiste saamiseks selle kohta, kuidas seda teha.</span><span class="sxs-lookup"><span data-stu-id="8ad84-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="8ad84-109">**Kasutaja litsentsi tüüp kehtetu või kasutaja nimi ei tuvastata:** Kasutajale tuleb määrata Intune ' i või EMS-i litsents.</span><span class="sxs-lookup"><span data-stu-id="8ad84-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="8ad84-110">Vaadake üle need dokumendid litsentsi määramiseks: [Office ' i halduskeskus](https://docs.microsoft.com/intune/licenses-assign) või [Azure ' i portaal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="8ad84-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="8ad84-111">Täiendavad ressursid probleemi lahendamiseks:</span><span class="sxs-lookup"><span data-stu-id="8ad84-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="8ad84-112">Levinud registreerimise tõrgete diagnoosimiseks ja lahendamiseks kasutage [tõrkeotsingu portaali Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) .</span><span class="sxs-lookup"><span data-stu-id="8ad84-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="8ad84-113">Vaadake [seda dokumenti](https://docs.microsoft.com/intune/help-desk-operators) rohkem üksikasju.</span><span class="sxs-lookup"><span data-stu-id="8ad84-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="8ad84-114">Vaadake need dokumendid läbi levinud tõrgete loendi, mis takistavad registreerimise ja resolutsioonide iga: [tõrkeotsingu juhend](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ja [tõrkeotsingu doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="8ad84-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="8ad84-115">[Teave selle kohta, kuidas registreeruda iOS-i seadmeid Microsoft Intune ' is](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="8ad84-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

