---
title: Microsofti Intune ' is olevate Android-seadmetega seotud probleemide tõrkeotsing
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759616"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="03528-102">Microsofti Intune ' is olevate Android-seadmetega seotud probleemide tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="03528-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="03528-103">Vaadake allpool loetletud ressursid probleemi lahendamiseks kohe.</span><span class="sxs-lookup"><span data-stu-id="03528-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="03528-104">Mõned levinud probleemid ja lahendus järgmiselt:</span><span class="sxs-lookup"><span data-stu-id="03528-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="03528-105">**Seade pole krüptitud tõrge ettevõtteportaalis:** Androidi uuemad versioonid, eriti alates v 7.0, nõuavad käivituspääsukoodi veendumaks, et teie seade on täielikult krüpteeritud.</span><span class="sxs-lookup"><span data-stu-id="03528-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="03528-106">Levinud lahendused on lubada käivituspin või täielikult krüptida seade.</span><span class="sxs-lookup"><span data-stu-id="03528-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="03528-107">Vaadake [seda dokumenti](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) lisateabe saamiseks.</span><span class="sxs-lookup"><span data-stu-id="03528-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="03528-108">**Seadmed ei saa sisse möllimist Intune teenus või Kuva "Unhealthy" Intune konsoolis:** Mõned Samsung 4,4 ja 5,5 seadmed ei pruugi teenuse sisse mölanda.</span><span class="sxs-lookup"><span data-stu-id="03528-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="03528-109">On 3 võimalikud lahendused sellele probleemile:</span><span class="sxs-lookup"><span data-stu-id="03528-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="03528-110">Avage käsitsi rakenduse Intune Company portaal, mis alustab automaatselt seadme sünkroonimist.</span><span class="sxs-lookup"><span data-stu-id="03528-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="03528-111">Värskendage seade Android 6,0 või uuem versioon.</span><span class="sxs-lookup"><span data-stu-id="03528-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="03528-112">Keelake Samsung Smart Manager Intune ettevõtte portaali haldamine.</span><span class="sxs-lookup"><span data-stu-id="03528-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="03528-113">Vaadake [seda dokumenti](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) nende probleemide ja resolutsioonide kohta lisateabe saamiseks.</span><span class="sxs-lookup"><span data-stu-id="03528-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="03528-114">**Kasutaja litsentsi tüüp kehtetu** või **kasutaja nimi tundmatu tõrge:** kasutaja peab olema määratud Intune või EMS litsents.</span><span class="sxs-lookup"><span data-stu-id="03528-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="03528-115">Vaadake üle need dokumendid litsentsi määramiseks: Office ' i administreerimiskeskus või Azure ' i portaal.</span><span class="sxs-lookup"><span data-stu-id="03528-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="03528-116">Täiendavad ressursid probleemi lahendamiseks:</span><span class="sxs-lookup"><span data-stu-id="03528-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="03528-117">Levinud registreerimise tõrgete diagnoosimiseks ja lahendamiseks kasutage [tõrkeotsingu portaali Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) .</span><span class="sxs-lookup"><span data-stu-id="03528-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="03528-118">Vaadake [seda dokumenti](https://docs.microsoft.com/intune/help-desk-operators) rohkem üksikasju.</span><span class="sxs-lookup"><span data-stu-id="03528-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="03528-119">Vaadake [seda dokumenti](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) levinud tõrgete loendi, mis takistavad registreerimise ja resolutsioonide iga.</span><span class="sxs-lookup"><span data-stu-id="03528-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="03528-120">[Vaadake, kuidas registreeruda Android-seadmeid Microsoft Intune ' is](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="03528-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
