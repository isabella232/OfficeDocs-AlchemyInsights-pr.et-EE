---
title: Microsoft Intune ' i Androidi seadmete registreerimisega seotud probleemide tõrkeotsing
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708994"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="cf705-102">Microsoft Intune ' i Androidi seadmete registreerimisega seotud probleemide tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="cf705-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="cf705-103">Probleemi lahendamiseks vaadake allpool loetletud ressursid üle.</span><span class="sxs-lookup"><span data-stu-id="cf705-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="cf705-104">Levinud probleemid ja lahendamise juhised.</span><span class="sxs-lookup"><span data-stu-id="cf705-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="cf705-105">**Seadmes pole krüptitud tõrget ettevõtte portaalis.** Androidi uuemad versioonid, eriti alates v 7.0-st, vajavad käivituse pääsukoodi, et veenduda, kas teie seade on täielikult krüptitud.</span><span class="sxs-lookup"><span data-stu-id="cf705-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="cf705-106">Levinumad lahendused on lubada käivitamise PIN-koodi või seadme täielikku krüptimist.</span><span class="sxs-lookup"><span data-stu-id="cf705-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="cf705-107">Lisateabe saamiseks lugege [see dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) üle.</span><span class="sxs-lookup"><span data-stu-id="cf705-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="cf705-108">**Seadmed ei suuda sisse logida Intune ' i teenusega või kuvada Intune ' i konsoolis "ebatervis".** Mõned Samsungi 4,4 ja 5,5 seadmed ei pruugi teenust sisse möllida.</span><span class="sxs-lookup"><span data-stu-id="cf705-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="cf705-109">Sellele probleemile on kolm võimalikku lahendust.</span><span class="sxs-lookup"><span data-stu-id="cf705-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="cf705-110">Avage käsitsi Intune ' i ettevõtte portaali rakendus, mis käivitab automaatselt seadme sünkroonimise.</span><span class="sxs-lookup"><span data-stu-id="cf705-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="cf705-111">Värskendage seadet Androidi 6,0 või uuema versiooniga.</span><span class="sxs-lookup"><span data-stu-id="cf705-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="cf705-112">Keelake Samsung Smart Manager Intune ettevõtte portaali haldamisel.</span><span class="sxs-lookup"><span data-stu-id="cf705-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="cf705-113">Vaadake üle [selle dokumendi](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) Lisateavet nende probleemide ja resolutsioonide kohta.</span><span class="sxs-lookup"><span data-stu-id="cf705-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="cf705-114">**Kasutaja litsentsi tüüp on vigane** või **kasutaja nimi pole tuvastanud tõrge:** kasutajale tuleb määrata Intune või EMS-i litsents.</span><span class="sxs-lookup"><span data-stu-id="cf705-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="cf705-115">Vaadake need dokumendid üle, et määrata litsents: Office halduskeskus või Azure ' i portaal.</span><span class="sxs-lookup"><span data-stu-id="cf705-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="cf705-116">Probleemi lahendamiseks täiendavad ressursid.</span><span class="sxs-lookup"><span data-stu-id="cf705-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="cf705-117">Saate kasutada [Intune tõrkeotsingu portaali](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) levinud liitumise tõrgete diagnoosimiseks ja lahendamiseks.</span><span class="sxs-lookup"><span data-stu-id="cf705-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="cf705-118">Lisateabe saamiseks vaadake [seda dokumenti](https://docs.microsoft.com/intune/help-desk-operators) üle.</span><span class="sxs-lookup"><span data-stu-id="cf705-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="cf705-119">Vaadake üle [see dokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) levinud tõrgete loend, mis takistavad iga kasutaja registreerimist ja eraldusvõimet.</span><span class="sxs-lookup"><span data-stu-id="cf705-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="cf705-120">[Siit saate teada, kuidas Microsoft Intune ' is Androidi seadmeid registreerida](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="cf705-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
