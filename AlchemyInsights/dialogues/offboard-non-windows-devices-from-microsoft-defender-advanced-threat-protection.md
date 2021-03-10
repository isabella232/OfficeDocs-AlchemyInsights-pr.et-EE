---
title: Microsoft Defenderi Offboard mitte-Windowsi seadmete täiustatud ohu kaitse (ATP)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693094"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="7141e-102">Microsoft Defenderi Offboard mitte-Windowsi seadmete täiustatud ohu kaitse (ATP)</span><span class="sxs-lookup"><span data-stu-id="7141e-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="7141e-103">Tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="7141e-103">Here's how:</span></span>

1. <span data-ttu-id="7141e-104">Kolmanda osapoole lahenduse katkestamiseks Microsoft Defenderi ATP-st järgige kolmanda osapoole dokumentatsiooni.</span><span class="sxs-lookup"><span data-stu-id="7141e-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="7141e-105">Eemaldage oma Azure Active Directory rentniku jaoks muu tootja lahenduse jaoks vajalikud load.</span><span class="sxs-lookup"><span data-stu-id="7141e-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="7141e-106">Logige sisse [Azure ' i portaali](https://go.microsoft.com/fwlink/?linkid=2125612).</span><span class="sxs-lookup"><span data-stu-id="7141e-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="7141e-107">Valige **kõik teenused**  >  **Azure Active Directory Enterprise ' i**  >  **rakendused**.</span><span class="sxs-lookup"><span data-stu-id="7141e-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="7141e-108">Valige offboard rakendus.</span><span class="sxs-lookup"><span data-stu-id="7141e-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="7141e-109">Valige **Kustuta**.</span><span class="sxs-lookup"><span data-stu-id="7141e-109">Select **Delete**.</span></span>

<span data-ttu-id="7141e-110">Lisateavet leiate teemast [Offboard mitte-Windowsi seadmed](https://go.microsoft.com/fwlink/?linkid=2143630).</span><span class="sxs-lookup"><span data-stu-id="7141e-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
