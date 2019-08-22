---
title: Tõrkeotsingu kasutamine Microsoft Intune Android seadmete
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 1e1d50c31df588a3416d758d40fbd7bde3f73b21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500067"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="66b99-102">Tõrkeotsingu kasutamine Microsoft Intune Android seadmete</span><span class="sxs-lookup"><span data-stu-id="66b99-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="66b99-103">Läbi nende lahendamiseks nüüd allpool loetletud ressurssidele.</span><span class="sxs-lookup"><span data-stu-id="66b99-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="66b99-104">Mõned levinud probleemid ja lahendus:</span><span class="sxs-lookup"><span data-stu-id="66b99-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="66b99-105">**Seadme krüptimata Ettevõtjaportaal viga:** Android, eriti alates v7.0, uuemad versioonid nõuavad pääsukoodi käivitamisel veenduge, et seade on täielikult krüptitud.</span><span class="sxs-lookup"><span data-stu-id="66b99-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="66b99-106">Käivituse PIN-koodi või täielikult seadme krüptimine on ühiseid lahendusi.</span><span class="sxs-lookup"><span data-stu-id="66b99-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="66b99-107">Läbi [selle dokumendi](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) lisateabe.</span><span class="sxs-lookup"><span data-stu-id="66b99-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="66b99-108">**Seadmed ei saate Intune service sisse või kuvada Intune konsoolis "Unhealthy":** Mõned Samsung 4.4 ja 5,5 seadmed võivad kontrolli teenindusse.</span><span class="sxs-lookup"><span data-stu-id="66b99-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="66b99-109">Seal on 3 võimalikud lahendused selle probleemi:</span><span class="sxs-lookup"><span data-stu-id="66b99-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="66b99-110">Käsitsi avada Intune Ettevõtjaportaal app, mis algatab automaatselt seadme sünkroonimine.</span><span class="sxs-lookup"><span data-stu-id="66b99-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="66b99-111">Värskendage seadme Android 6.0 või kõrgem.</span><span class="sxs-lookup"><span data-stu-id="66b99-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="66b99-112">Keelata Samsung Smart Manager hallata Intune'i Ettevõtjaportaal.</span><span class="sxs-lookup"><span data-stu-id="66b99-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="66b99-113">Läbi [selle dokumendi](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) täpsemat teavet need probleemid ja lahendused.</span><span class="sxs-lookup"><span data-stu-id="66b99-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="66b99-114">**Kasutaja litsentsi tüüp ei sobi** või **kasutaja nimi tundmatu tõrge:** kasutaja peab olema määratud Intune või EMS litsentsi.</span><span class="sxs-lookup"><span data-stu-id="66b99-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="66b99-115">Läbi nende dokumentide kaudu litsentsi omistamiseks: Office administreerimiskeskuse või Azure portaali.</span><span class="sxs-lookup"><span data-stu-id="66b99-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="66b99-116">Lisaressursse, mis probleemi lahendada:</span><span class="sxs-lookup"><span data-stu-id="66b99-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="66b99-117">Diagnoosimiseks ja lahendamiseks ühise registreerimise rikete [Intune tõrkeotsingu portaali](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) abil.</span><span class="sxs-lookup"><span data-stu-id="66b99-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="66b99-118">Läbi [selle dokumendi](https://docs.microsoft.com/intune/help-desk-operators) lisateabe saamiseks.</span><span class="sxs-lookup"><span data-stu-id="66b99-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="66b99-119">Nimekiri kõige sagedasemad vead, mis takistavad registreerimine ja lahendused igale [dokumendi](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) läbivaatamiseks.</span><span class="sxs-lookup"><span data-stu-id="66b99-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="66b99-120">[Kuidas registreeruda Microsoft Intune Androidiga](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="66b99-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
