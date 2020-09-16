---
title: Seadme laoseisu häälestamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667874"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="b3831-102">Seadme laoseisu häälestamine</span><span class="sxs-lookup"><span data-stu-id="b3831-102">Intune Device Inventory</span></span>

<span data-ttu-id="b3831-103">Seadmete Blade annab haldurile ülevaate halduses olevatest seadmetest, mida saab seadme põhjal häälestada.</span><span class="sxs-lookup"><span data-stu-id="b3831-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="b3831-104">Kuvatud teave sisaldab: riistvara, avastatud rakendusi, seadme nõuetele vastavuse olekut ja seadme konfigureerimise olekut.</span><span class="sxs-lookup"><span data-stu-id="b3831-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="b3831-105">Riistvara ja avastatud rakenduste laoseisu andmed kogutakse seitsme päeva jooksul.</span><span class="sxs-lookup"><span data-stu-id="b3831-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="b3831-106">Teatatud riistvara rakendused ja konkreetsed elemendid erinevad olenevalt seadme opsüsteemist ja sellest, kas seade on ise või ettevõtte omanduses.</span><span class="sxs-lookup"><span data-stu-id="b3831-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="b3831-107">Lisateavet leiate teemast [seadme üksikasjade kuvamine Intune ' is](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="b3831-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="b3831-108">**KKK**</span><span class="sxs-lookup"><span data-stu-id="b3831-108">**FAQ**</span></span>

<span data-ttu-id="b3831-109">K: ma ei saa täieliku laoseisu taotluste loendit Windowsi seadmetes.</span><span class="sxs-lookup"><span data-stu-id="b3831-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="b3831-110">Miks mitte?</span><span class="sxs-lookup"><span data-stu-id="b3831-110">Why not?</span></span>

<span data-ttu-id="b3831-111">V: praegu on ainult moodsad rakendused loetletud Windows 10 arvutites, mis on tähistatud ettevõtte seadmetena.</span><span class="sxs-lookup"><span data-stu-id="b3831-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="b3831-112">Intune ei kogu teavet nendesse seadmetesse installitud Win32 rakenduste kohta.</span><span class="sxs-lookup"><span data-stu-id="b3831-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="b3831-113">K: Miks ei koguta telefoninumbreid kõigilt seadmetelt?</span><span class="sxs-lookup"><span data-stu-id="b3831-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="b3831-114">V: telefonid, mis on kategoriseeritud kui ettevõtte seadmed Intune ' is, ei ole määratud nende täieliku telefoninumbriga, kui käivitate näiteks mobiilsideseadme laovarude aruandeid.</span><span class="sxs-lookup"><span data-stu-id="b3831-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="b3831-115">Bring-you-oma-seadme telefoninumbrid on alati osaliselt maskid tärnide (\* \* \* \*) ja näidata ainult neli viimast numbrit.</span><span class="sxs-lookup"><span data-stu-id="b3831-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>