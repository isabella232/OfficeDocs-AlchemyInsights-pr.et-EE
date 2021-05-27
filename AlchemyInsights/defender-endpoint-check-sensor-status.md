---
title: Defenderi lõpp-punkti kontrolli anduri olek
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676182"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="e4d93-102">Defenderi lõpp-punkti kontrolli anduri olek</span><span class="sxs-lookup"><span data-stu-id="e4d93-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="e4d93-103">**Anduriprobleemidega seadmed** asuvad turbetoimingute armatuurlaual.</span><span class="sxs-lookup"><span data-stu-id="e4d93-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="e4d93-104">See paan annab teavet selle kohta, kuidas seade saab anda anduriandmeid ja suhelda Teenusega Defender for Endpoint.</span><span class="sxs-lookup"><span data-stu-id="e4d93-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="e4d93-105">Selles kirjeldatakse, kui palju seadmeid vajab tähelepanu ja aitab teil probleemsed seadmed tuvastada ja teadaolevate probleemide lahendamiseks midagi ette võtta.</span><span class="sxs-lookup"><span data-stu-id="e4d93-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="e4d93-106">Paanil on kaks olekunäidikut, mis annavad teavet selle kohta, kui palju seadmeid ei teavitata teenusest õigesti.</span><span class="sxs-lookup"><span data-stu-id="e4d93-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="e4d93-107">**Valesti konfigureeritud** Seadmed, mis võivad osaliselt anduriandmeid teenusele Defender for Endpoint esitada ja mis võivad konfiguratsioonivigu parandada.</span><span class="sxs-lookup"><span data-stu-id="e4d93-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="e4d93-108">**Passiivne** Seadmed, mis on viimase kuu jooksul lõpetanud aruandluse Teenusele Defender for Endpoint rohkem kui seitse päeva.</span><span class="sxs-lookup"><span data-stu-id="e4d93-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="e4d93-109">Kui klõpsate mõnda rühma, suunab see teid loendisse Seadmed, mis on filtreeritud vastavalt teie valikutele.</span><span class="sxs-lookup"><span data-stu-id="e4d93-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="e4d93-110">Loendis Seadmed saate seisundioleku loendit filtreerida järgmise oleku järgi.</span><span class="sxs-lookup"><span data-stu-id="e4d93-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="e4d93-111">**Aktiivne** Seadmed, mis suhtlevad aktiivselt teenusega Defender for Endpoint.</span><span class="sxs-lookup"><span data-stu-id="e4d93-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="e4d93-112">**Valesti konfigureeritud** Seadmed, mis võivad osaliselt anduriandmeid teenusele Defender for Endpoint esitada, kuid mille konfiguratsioonitõrked tuleb parandada.</span><span class="sxs-lookup"><span data-stu-id="e4d93-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="e4d93-113">Valesti konfigureeritud seadmetel võib olla üks või mitme järgmise probleemi kombinatsioon.</span><span class="sxs-lookup"><span data-stu-id="e4d93-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="e4d93-114">Anduriandmeid pole . Seadmed on sensorandmete saatmise lõpetanud.</span><span class="sxs-lookup"><span data-stu-id="e4d93-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="e4d93-115">Piiratud teatisi saab seadmest käivitada.</span><span class="sxs-lookup"><span data-stu-id="e4d93-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="e4d93-116">Kommunikatsioonihäired – seadmega suhtlemine on häiritud.</span><span class="sxs-lookup"><span data-stu-id="e4d93-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="e4d93-117">Failide saatmine süvaanalüüsiks, failide blokeerimiseks, seadme isoleerimiseks võrgust ja muud toimingud, mis nõuavad seadmega suhtlemist, ei pruugi töötada.</span><span class="sxs-lookup"><span data-stu-id="e4d93-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="e4d93-118">**Passiivne** Seadmed, mis on lõpetanud aruandluse Teenusele Defender for Endpoint.</span><span class="sxs-lookup"><span data-stu-id="e4d93-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="e4d93-119">Kogu loendi saate alla laadida CSV-vormingus, kasutades ekspordifunktsiooni.</span><span class="sxs-lookup"><span data-stu-id="e4d93-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="e4d93-120">Lisateavet leiate teemast [Sensori seisundi seisundi kontrollimine rakenduses Microsoft Defender for Endpoint.](/microsoft-365/security/defender-endpoint/check-sensor-status)</span><span class="sxs-lookup"><span data-stu-id="e4d93-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="e4d93-121">Lisateavet selle kohta, mis põhjustas seadme passiivseks või valesti konfigureerimise, leiate teemast Ebatervislike andurite lahendus [Rakenduses Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span><span class="sxs-lookup"><span data-stu-id="e4d93-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
