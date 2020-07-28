---
title: Andmete eemaldamine ja seadmete eemaldamine Intune kaudu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439155"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="e1545-102">Andmete eemaldamine ja seadmete eemaldamine Intune kaudu</span><span class="sxs-lookup"><span data-stu-id="e1545-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="e1545-103">Seade on kasutuselt kõrvaldatud ja seadme tühjendamiseks saab kasutada ettevõtte andmeid, mida hallatakse Intune abil või tehase lähtestamiseks ja seadme vaikesätetele tagastamiseks.</span><span class="sxs-lookup"><span data-stu-id="e1545-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="e1545-104">Logige sisse rakendusse Microsoft 365 Device Management ja valige **seadmed**  >  **kõigis seadmetes**.</span><span class="sxs-lookup"><span data-stu-id="e1545-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="e1545-105">Valige seade, mille soovite kustutada.</span><span class="sxs-lookup"><span data-stu-id="e1545-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="e1545-106">Valige eemaldatava kaugjuhtimispuldi tüüp.</span><span class="sxs-lookup"><span data-stu-id="e1545-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="e1545-107">Pensionile kustutab ainult ettevõtte andmed, samal ajal kui täielikud salvrätikud taastavad seadme tehase seadetesse.</span><span class="sxs-lookup"><span data-stu-id="e1545-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="e1545-108">Kinnitamiseks valige **Jah** .</span><span class="sxs-lookup"><span data-stu-id="e1545-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="e1545-109">Kui pühkimine on lõpule jõudnud, kuvatakse seadme toimingu olekuks Ootel.</span><span class="sxs-lookup"><span data-stu-id="e1545-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="e1545-110">Kui toiming on lõpule viidud, ei näe te hallatava seadme loendis enam mobiilsideseadmet.</span><span class="sxs-lookup"><span data-stu-id="e1545-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="e1545-111">**Märkus** Ettevõtte andmeid ei saa eemaldada Azure AD-ga ühendatud seadmetest.</span><span class="sxs-lookup"><span data-stu-id="e1545-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="e1545-112">Lisateavet selle kohta, kuidas eemaldada ja kustutada toiminguid, sealhulgas seda, mis jääb alles ja mis kustutatakse, leiate teemast [seadmete eemaldamine, kui kasutate seadme tühjendamise, pensionile jäämist või käsitsi registreerimise tühistamist](https://docs.microsoft.com/intune/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="e1545-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="e1545-113">Kui soovite kustutada kõik macOS-seadme andmed, lugege teemat [kõigi andmete kustutamine MacOS-seadmest](https://docs.microsoft.com/intune/device-erase).</span><span class="sxs-lookup"><span data-stu-id="e1545-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>