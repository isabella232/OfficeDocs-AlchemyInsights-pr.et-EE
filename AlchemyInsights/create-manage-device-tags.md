---
title: Seadmesiltide või -rühmade loomine ja haldamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731450"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="4a5c5-102">Seadmesiltide või -rühmade loomine ja haldamine</span><span class="sxs-lookup"><span data-stu-id="4a5c5-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="4a5c5-103">Loogiliste rühmade kuuluvuse loomiseks saate lisada seadmetes silte.</span><span class="sxs-lookup"><span data-stu-id="4a5c5-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="4a5c5-104">Seadmesildid toetavad võrgu õiget vastendamist, võimaldades teil manustada erinevaid silte konteksti jäädvustamiseks ja dünaamilise loendi loomise lubamiseks juhtumi osana.</span><span class="sxs-lookup"><span data-stu-id="4a5c5-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="4a5c5-105">Silte saab kasutada filtrina loendivaates Seadmed või seadmete rühmitamiseks.</span><span class="sxs-lookup"><span data-stu-id="4a5c5-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="4a5c5-106">Lisateavet seadme rühmitamise kohta leiate teemast [Seadmesiltide loomine ja haldamine.](/microsoft-365/security/defender-endpoint/machine-tags)</span><span class="sxs-lookup"><span data-stu-id="4a5c5-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="4a5c5-107">Siltide lisamiseks seadmetesse saate teha:</span><span class="sxs-lookup"><span data-stu-id="4a5c5-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="4a5c5-108">Portaali kasutamine</span><span class="sxs-lookup"><span data-stu-id="4a5c5-108">Using the portal</span></span>

- <span data-ttu-id="4a5c5-109">Registrivõtme väärtuse seadmine</span><span class="sxs-lookup"><span data-stu-id="4a5c5-109">Setting a registry key value</span></span>
 
<span data-ttu-id="4a5c5-110">**Märkus.** Sildi seadmesse lisamist ja selle kättesaadavust seadmete loendis ja seadmelehel võib olla latentsusaeg.</span><span class="sxs-lookup"><span data-stu-id="4a5c5-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="4a5c5-111">Api abil seadmesiltide lisamiseks lugege teemat [Seadmesiltide API lisamine või eemaldamine.](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags)</span><span class="sxs-lookup"><span data-stu-id="4a5c5-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="4a5c5-112">Seadmesiltide lisamine ja haldamine portaali abil</span><span class="sxs-lookup"><span data-stu-id="4a5c5-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="4a5c5-113">Valige seade, kus soovite silte hallata.</span><span class="sxs-lookup"><span data-stu-id="4a5c5-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="4a5c5-114">Saate valida või otsida seadet mis tahes järgmistest vaadetest.</span><span class="sxs-lookup"><span data-stu-id="4a5c5-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="4a5c5-115">**Turbetoimingute armatuurlaud** Valige jaotises Aktiivsete teatistega ülemised seadmed seadme nimi.</span><span class="sxs-lookup"><span data-stu-id="4a5c5-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="4a5c5-116">**Teatiste** järjekord – valige teatejärjekorras seadme ikooni kõrval seadme nimi.</span><span class="sxs-lookup"><span data-stu-id="4a5c5-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="4a5c5-117">**Seadmete loend** – valige seadmete loendist seadme nimi.</span><span class="sxs-lookup"><span data-stu-id="4a5c5-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="4a5c5-118">**Otsinguväli** – valige rippmenüüst Seade ja sisestage seadme nimi.</span><span class="sxs-lookup"><span data-stu-id="4a5c5-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="4a5c5-119">Teatiselehele pääsete ka faili ja IP-vaadete kaudu.</span><span class="sxs-lookup"><span data-stu-id="4a5c5-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="4a5c5-120">Valige **vastusetoimingute** reast Käsk Halda silte.</span><span class="sxs-lookup"><span data-stu-id="4a5c5-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="4a5c5-121">Siltide otsimiseks või loomiseks tippige.</span><span class="sxs-lookup"><span data-stu-id="4a5c5-121">Type to find or create tags.</span></span>

<span data-ttu-id="4a5c5-122">Sildid lisatakse seadmevaatesse ja kajastuvad loendivaates Seadmed.</span><span class="sxs-lookup"><span data-stu-id="4a5c5-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="4a5c5-123">Seejärel saate kasutada filtrit Sildid, et näha asjakohast seadmete loendit.</span><span class="sxs-lookup"><span data-stu-id="4a5c5-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="4a5c5-124">Lisateavet leiate teemast [Seadmesiltide loomine ja haldamine.](/microsoft-365/security/defender-endpoint/machine-tags)</span><span class="sxs-lookup"><span data-stu-id="4a5c5-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>