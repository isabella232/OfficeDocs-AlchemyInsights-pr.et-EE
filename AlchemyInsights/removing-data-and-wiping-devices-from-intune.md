---
title: Andmete eemaldamine ja seadmete tühjendamine Intune‘i kaudu
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
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416309"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="48b4d-102">Andmete eemaldamine ja seadmete tühjendamine Intune‘i kaudu</span><span class="sxs-lookup"><span data-stu-id="48b4d-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="48b4d-103">Seadme kasutuselt kõrvaldamise ja seadme tühjendamise kaugtoimingutega saab eemaldada Intune‘i hallatavad ettevõtteandmed või lähtestada seadme vaikesätted.</span><span class="sxs-lookup"><span data-stu-id="48b4d-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="48b4d-104">Logige sisse Microsoft 365 seadmehaldusesse ja valige **Seadmed** > **Kõik seadmed**.</span><span class="sxs-lookup"><span data-stu-id="48b4d-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="48b4d-105">Valige seade, millest soovite sisu kustutada.</span><span class="sxs-lookup"><span data-stu-id="48b4d-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="48b4d-106">Valige soovitud kaugkustutamise tüüp.</span><span class="sxs-lookup"><span data-stu-id="48b4d-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="48b4d-107">Kasutuselt kõrvaldamise korral kustutatakse ainult asutuse teave; täielikul tühjendamisel taastatakse seadmes algsätted.</span><span class="sxs-lookup"><span data-stu-id="48b4d-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="48b4d-108">Kinnitamiseks valige **Jah**.</span><span class="sxs-lookup"><span data-stu-id="48b4d-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="48b4d-109">Kuni tühjenduse lõpulejõudmiseni kuvatakse seadme toimingu olekuna *Kasutuselt kõrvaldamise ootel*.</span><span class="sxs-lookup"><span data-stu-id="48b4d-109">Until the wipe finishes, the Device action status shows as *Retire Pending*.</span></span>
    <span data-ttu-id="48b4d-110">Pärast toimingu lõpulejõudmist ei kuvata seda nutiseadet enam hallatavate seadmete loendis.</span><span class="sxs-lookup"><span data-stu-id="48b4d-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

> [!NOTE]
> <span data-ttu-id="48b4d-111">Ettevõtte andmeid ei saa eemaldada seadmetest, mis on liidetud Azure AD-ga.</span><span class="sxs-lookup"><span data-stu-id="48b4d-111">Company data can't be removed from devices JOINED to Azure AD.</span></span> 

<span data-ttu-id="48b4d-112">Kasutuselt kõrvaldamise ja tühjendamise toimingute täielikud üksikasjad (sh teabe selle kohta, mis hoitakse alles ja mis kustutatakse) leiate järgmisest dokumentatsioonist:</span><span class="sxs-lookup"><span data-stu-id="48b4d-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see following documentation:</span></span>

- <span data-ttu-id="48b4d-113">[Seadmete eemaldamine tühjendamise, kasutuselt kõrvaldamise või registrist käsitsi kustutamisega](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="48b4d-113">[Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span></span>
- [<span data-ttu-id="48b4d-114">Ainult ettevõtteandmete kustutamine Intune‘i hallatavatest rakendustest</span><span class="sxs-lookup"><span data-stu-id="48b4d-114">How to wipe only corporate data from Intune-managed apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- <span data-ttu-id="48b4d-115">[Kõigi andmete kustutamine macOS-i seadmest](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span><span class="sxs-lookup"><span data-stu-id="48b4d-115">[Erase all data from a macOS device](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span></span>