---
title: Probleemid seadme varudest välja lülitatud või kasutuselt kõrvaldatud seadme eemaldamisega
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/11/2021
ms.locfileid: "52564170"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="e6b2e-102">Probleemid seadme varudest välja lülitatud või kasutuselt kõrvaldatud seadme eemaldamisega</span><span class="sxs-lookup"><span data-stu-id="e6b2e-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="e6b2e-103">Microsoft Defender lõpp-punkti jaoks ei võimalda praegu seadme varudest eemaldada seadmekirjet, mis on seadmest maha lülitatud või kasutuselt kõrvaldatud.</span><span class="sxs-lookup"><span data-stu-id="e6b2e-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="e6b2e-104">Turvalisuse huvides jääb seade portaali ajalookirjeks kuni 180 päevaks.</span><span class="sxs-lookup"><span data-stu-id="e6b2e-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="e6b2e-105">Kuid seadme andmed likvideeritakse vastavalt teie konfigureeritud säilitusperioodile.</span><span class="sxs-lookup"><span data-stu-id="e6b2e-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="e6b2e-106">**Märkus.** Välja lülitatud või kasutuselt kõrvaldatud seade  lülitub seitsme päeva pärast automaatselt olekusse Passiivne.</span><span class="sxs-lookup"><span data-stu-id="e6b2e-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="e6b2e-107">Lisaks ei arvestata viimase 30 päeva jooksul aktiivseid seadmeid andmetesse, mis peegeldavad teie ettevõtte ohu- ja nõrkusehaldus või Microsoft Secure Score for Devices.</span><span class="sxs-lookup"><span data-stu-id="e6b2e-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="e6b2e-108">Kui te ikka ei soovi seadme varude vaates teatud seadmeid näha, proovige seadme silti lisada, et filtreerida kasutuselt kõrvaldatud seade välja seadme varude vaatest.</span><span class="sxs-lookup"><span data-stu-id="e6b2e-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="e6b2e-109">Lisateavet leiate järgmistest teemadest.</span><span class="sxs-lookup"><span data-stu-id="e6b2e-109">For more information, see:</span></span>

[<span data-ttu-id="e6b2e-110">Offboard devices from the Microsoft Defender for Endpoint service</span><span class="sxs-lookup"><span data-stu-id="e6b2e-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="e6b2e-111">Säriskoor ohu- ja nõrkusehaldus</span><span class="sxs-lookup"><span data-stu-id="e6b2e-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="e6b2e-112">Ebatervislike andurite lahendus Microsoft Defenderi lõpp-punkti jaoks</span><span class="sxs-lookup"><span data-stu-id="e6b2e-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="e6b2e-113">Sildistamine tõhusalt (1. osa)</span><span class="sxs-lookup"><span data-stu-id="e6b2e-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="e6b2e-114">Sildistamine tõhusalt (2. osa)</span><span class="sxs-lookup"><span data-stu-id="e6b2e-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="e6b2e-115">Sildistamine tõhusalt (3. osa)</span><span class="sxs-lookup"><span data-stu-id="e6b2e-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




