---
title: Tarkvara inventuur puudub või on ebatäpne
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676263"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="c95cd-102">Tarkvara inventuur puudub või on ebatäpne</span><span class="sxs-lookup"><span data-stu-id="c95cd-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="c95cd-103">Tarkvara inventar ohu- ja nõrkusehaldus (TVM) on teie asutuse teadaolevate tarkvarade loend, kus on ametlikud ühise platvormi loendid (CPE).</span><span class="sxs-lookup"><span data-stu-id="c95cd-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="c95cd-104">Ilma ametliku CPE-ta tarkvaratoodetel pole avaldatud haavatavusi.</span><span class="sxs-lookup"><span data-stu-id="c95cd-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="c95cd-105">Laovaru sisaldab ka üksikasju( nt tarnija nime, puuduste arvu, ohte ja avatud seadmete arvu).</span><span class="sxs-lookup"><span data-stu-id="c95cd-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="c95cd-106">Seadmetes tehtud tarkvaramuudatused kajastuvad tavaliselt kahe tunni jooksul turbeportaalis.</span><span class="sxs-lookup"><span data-stu-id="c95cd-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="c95cd-107">Mõnikord võib see siiski kauem aega võtta.</span><span class="sxs-lookup"><span data-stu-id="c95cd-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="c95cd-108">Praegu ei saa sünkroonimist sundida. see on pidev hindamine.</span><span class="sxs-lookup"><span data-stu-id="c95cd-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="c95cd-109">Kui tegite tarkvaramuutuse ja muudatus ei kajastu TVM-is täpselt pärast 5 tundi, tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="c95cd-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="c95cd-110">Tarkvara tuvastamise kohta saate teavet tarkvara tõendusmaterjali jaotisest.</span><span class="sxs-lookup"><span data-stu-id="c95cd-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="c95cd-111">Veenduge, et tarkvara oleks toetatud.</span><span class="sxs-lookup"><span data-stu-id="c95cd-111">Make sure that the software is supported.</span></span> <span data-ttu-id="c95cd-112">Tarkvara võib olla nähtav ainult seadme tasemel isegi siis, kui see pole praegu ohu- ja nõrkusehaldus.</span><span class="sxs-lookup"><span data-stu-id="c95cd-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="c95cd-113">Siiski on saadaval ainult piiratud andmed.</span><span class="sxs-lookup"><span data-stu-id="c95cd-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="c95cd-114">Teavet portaali ebatäpsuste kohta leiate teemast Ebatäpsusest [teatamine.](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)</span><span class="sxs-lookup"><span data-stu-id="c95cd-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="c95cd-115">**Märkus.** Ebatäpsusest teatamine MDE portaalis on ühe suunaline kanal tehnikasse.</span><span class="sxs-lookup"><span data-stu-id="c95cd-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="c95cd-116">Kui probleem on pakiline, avage tugiteenuste pilet.</span><span class="sxs-lookup"><span data-stu-id="c95cd-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="c95cd-117">Lisateavet leiate teemast Tarkvara [inventuur – ohu- ja nõrkusehaldus](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span><span class="sxs-lookup"><span data-stu-id="c95cd-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>