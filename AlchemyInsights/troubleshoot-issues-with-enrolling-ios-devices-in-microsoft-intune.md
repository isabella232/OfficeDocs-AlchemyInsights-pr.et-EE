---
title: Microsoft Intune'is iOS-i seadmete registreerimisega seotud probleemide tõrkeotsing
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823459"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="68466-102">Microsoft Intune'is iOS-i seadmete registreerimisega seotud probleemide tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="68466-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="68466-103">Vaadake allpool loetletud ressursid üle, et probleem kohe lahendada.</span><span class="sxs-lookup"><span data-stu-id="68466-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="68466-104">Levinumad tõrketeated ja eraldusvõime juhised.</span><span class="sxs-lookup"><span data-stu-id="68466-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="68466-105">**Seadme suurtähelukk on saavutatud** Kasutajal on rohkem seadmeid, mis on registreeritud kui seadme limiit.</span><span class="sxs-lookup"><span data-stu-id="68466-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="68466-106">Vaadake need dokumendid [üle, et eemaldada seade](https://docs.microsoft.com/intune/devices-wipe) [või muuta seadme piirangut.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="68466-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="68466-107">**Seda teenust ei toetata. Registreerimispoliitika puudub.** Apple'i tõuketeatise teenus (APNS) tuleb konfigureerida või uuendada.</span><span class="sxs-lookup"><span data-stu-id="68466-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="68466-108">Vaadake [läbi see dokument,](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) et saada juhiseid selle kohta, kuidas seda teha.</span><span class="sxs-lookup"><span data-stu-id="68466-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="68466-109">**Kasutajalitsentsi tüüp On kehtetu või kasutajanime ei tuvastata.** Kasutajale tuleb määrata Intune'i või EMS-i litsents.</span><span class="sxs-lookup"><span data-stu-id="68466-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="68466-110">Vaadake need dokumendid üle, et määrata litsents [office'i halduskeskuse või](https://docs.microsoft.com/intune/licenses-assign) [Azure'i portaali kaudu.](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="68466-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="68466-111">Täiendavad ressursid probleemi lahendamiseks.</span><span class="sxs-lookup"><span data-stu-id="68466-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="68466-112">[Intune'i tõrkeotsinguportaali](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) abil saate diagnoosida ja lahendada levinumaid registreerimistõrkeid.</span><span class="sxs-lookup"><span data-stu-id="68466-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="68466-113">Lisateavet [leiate sellest](https://docs.microsoft.com/intune/help-desk-operators) dokumendist.</span><span class="sxs-lookup"><span data-stu-id="68466-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="68466-114">Vaadake need dokumendid üle, et saada ülevaade levinumatest vigadest, mis takistavad registreerimist ja lahendamist: tõrkeotsingu [juhend ja](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) [tõrkeotsingu dokument.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="68466-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="68466-115">[Siit saate teada, kuidas registreerida iOS-i seadmeid Microsoft Intune'is.](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="68466-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

