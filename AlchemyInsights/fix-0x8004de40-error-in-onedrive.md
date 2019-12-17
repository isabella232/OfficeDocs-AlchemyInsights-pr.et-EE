---
title: Fix 0x8004de40 tõrge OneDrive
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052033"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="da92d-102">Fix 0x8004de40 tõrge OneDrive</span><span class="sxs-lookup"><span data-stu-id="da92d-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="da92d-103">Kui saate tõrketeate 0x8004de40 OneDrive ' iga:</span><span class="sxs-lookup"><span data-stu-id="da92d-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="da92d-104">Taaskäivitage mõjutatud arvuti ajal, mis on ühendatud teie Võimeve Directory domeeniga.</span><span class="sxs-lookup"><span data-stu-id="da92d-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="da92d-105">Kui reboot ei lahenda probleemi, lahti ühendada ja ühendada oma seadme Azure AD.</span><span class="sxs-lookup"><span data-stu-id="da92d-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="da92d-106">**Märkus**: sa peaksid olema oma ettevõtte võrgus, tehes neid samme.</span><span class="sxs-lookup"><span data-stu-id="da92d-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="da92d-107">Ärge tehke neid samme, kui te ei saa luua ühendust oma ettevõtte infrastruktuuriga (nt reisil olles).</span><span class="sxs-lookup"><span data-stu-id="da92d-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="da92d-108">Avage administraatoriõigustega Käsuviip.</span><span class="sxs-lookup"><span data-stu-id="da92d-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="da92d-109">Laiendatud käsuviiba avamiseks klõpsake- **Start**, paremklõpsake **Käsuviip**ja seejärel klõpsake nuppu **Käivita administraatorina**.</span><span class="sxs-lookup"><span data-stu-id="da92d-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="da92d-110">Tippige *dsregcmd/Leave* ja vajutage sisestusklahvi **Enter**.</span><span class="sxs-lookup"><span data-stu-id="da92d-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="da92d-111">Kui olete valmis, tippige *dsregcmd/JOIN* ja vajutage sisestusklahvi **Enter**.</span><span class="sxs-lookup"><span data-stu-id="da92d-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="da92d-112">Kui olete valmis, sulgege Käsuviip.</span><span class="sxs-lookup"><span data-stu-id="da92d-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="da92d-113">Taaskäivitage arvuti ja logige OneDrive ' i sisse.</span><span class="sxs-lookup"><span data-stu-id="da92d-113">Reboot the computer, and log into OneDrive.</span></span>