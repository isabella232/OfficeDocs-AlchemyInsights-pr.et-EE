---
title: Microsoft Intune'is Androidi seadmete registreerimisega seotud probleemide tõrkeotsing
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830938"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="15438-102">Microsoft Intune'is Androidi seadmete registreerimisega seotud probleemide tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="15438-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="15438-103">Vaadake allpool loetletud ressursid üle, et probleem kohe lahendada.</span><span class="sxs-lookup"><span data-stu-id="15438-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="15438-104">Mõned levinumad probleemid ja lahendused.</span><span class="sxs-lookup"><span data-stu-id="15438-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="15438-105">**Seadmes pole krüptitud tõrge ettevõtteportaalis.** Androidi uuemad versioonid, eriti alates versioonist v7.0, nõuavad käivituspääsukoodi, et veenduda, et teie seade on täielikult krüptitud.</span><span class="sxs-lookup"><span data-stu-id="15438-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="15438-106">Levinud lahendused on lubada käivitusviga või krüptida seade täielikult.</span><span class="sxs-lookup"><span data-stu-id="15438-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="15438-107">Lisateavet [leiate sellest](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) dokumendist.</span><span class="sxs-lookup"><span data-stu-id="15438-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="15438-108">Seadmetel ei õnnestu Intune'i teenusega sisse logida või intune'i halduskonsoolis kuvatakse **"Ebatervislik".** Mõned Samsung 4.4 ja 5.5 seadmed ei pruugi teenusesse sisseregistreerida.</span><span class="sxs-lookup"><span data-stu-id="15438-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="15438-109">Sellele probleemile on kolm võimalikku lahendust.</span><span class="sxs-lookup"><span data-stu-id="15438-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="15438-110">Avage intune'i ettevõtteportaali rakendus käsitsi, mis algatab automaatselt seadme sünkroonimise.</span><span class="sxs-lookup"><span data-stu-id="15438-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="15438-111">Värskendage seade versioonile Android 6.0 või uuem.</span><span class="sxs-lookup"><span data-stu-id="15438-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="15438-112">Keelake Samsung Smart Manager intune'i ettevõtteportaali haldamisel.</span><span class="sxs-lookup"><span data-stu-id="15438-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="15438-113">Vaadake [see dokument läbi,](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) et lisateavet nende probleemide ja lahenduste kohta.</span><span class="sxs-lookup"><span data-stu-id="15438-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="15438-114">**Kasutajalitsentsi tüübi kehtetu** või tundmatu kasutajanime **tõrge:** kasutajale tuleb määrata Intune'i või EMS-i litsents.</span><span class="sxs-lookup"><span data-stu-id="15438-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="15438-115">Vaadake need dokumendid üle, et määrata litsents office'i halduskeskuse või Azure'i portaali kaudu.</span><span class="sxs-lookup"><span data-stu-id="15438-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="15438-116">Täiendavad ressursid probleemi lahendamiseks.</span><span class="sxs-lookup"><span data-stu-id="15438-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="15438-117">[Intune'i tõrkeotsinguportaali](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) abil saate diagnoosida ja lahendada levinumaid registreerimistõrkeid.</span><span class="sxs-lookup"><span data-stu-id="15438-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="15438-118">Lisateavet [leiate sellest](https://docs.microsoft.com/intune/help-desk-operators) dokumendist.</span><span class="sxs-lookup"><span data-stu-id="15438-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="15438-119">Vaadake [see dokument üle,](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) et saada ülevaade levinumatest vigadest, mis takistavad igale dokumendile registreerimist ja lahendamist.</span><span class="sxs-lookup"><span data-stu-id="15438-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="15438-120">[Siit saate teada, kuidas registreeruda Microsoft Intune'is Androidi seadmeid.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="15438-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
