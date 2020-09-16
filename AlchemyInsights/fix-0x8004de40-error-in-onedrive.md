---
title: OneDrive ' i 0x8004de40 lahendamise tõrge
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745126"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="4210a-102">OneDrive ' i 0x8004de40 lahendamise tõrge</span><span class="sxs-lookup"><span data-stu-id="4210a-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="4210a-103">Kui OneDrive ' iga kuvatakse 0x8004de40 tõrge, tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="4210a-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="4210a-104">Taaskäivitage mõjutatud arvuti, kui olete ühendatud oma Acitve kataloogiteenuse domeeniga.</span><span class="sxs-lookup"><span data-stu-id="4210a-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="4210a-105">Kui taaskäivitamine probleemi ei lahenda, liituge oma seadmega Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4210a-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="4210a-106">**Märkus**: te peate nende toimingute tegemisel olema ettevõtte võrgus.</span><span class="sxs-lookup"><span data-stu-id="4210a-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="4210a-107">Ärge tehke neid toiminguid, kui te ei saa luua ühendust oma ettevõtte infrastruktuuriga (nt reisil olles).</span><span class="sxs-lookup"><span data-stu-id="4210a-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="4210a-108">Avage tõstetud Käsuviip.</span><span class="sxs-lookup"><span data-stu-id="4210a-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="4210a-109">Kõrgenenud käsuviiba avamiseks klõpsake nuppu **Start**, paremklõpsake käsku **Käsuviip**ja seejärel klõpsake käsku **Käivita administraatorina**.</span><span class="sxs-lookup"><span data-stu-id="4210a-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="4210a-110">Tippige *dsregcmd/Leave* ja vajutage sisestusklahvi ( **Enter)**.</span><span class="sxs-lookup"><span data-stu-id="4210a-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="4210a-111">Kui olete lõpetanud, tippige *dsregcmd/JOIN* ja vajutage sisestusklahvi ( **Enter)**.</span><span class="sxs-lookup"><span data-stu-id="4210a-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="4210a-112">Kui olete lõpetanud, sulgege Käsuviip.</span><span class="sxs-lookup"><span data-stu-id="4210a-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="4210a-113">Taaskäivitage arvuti ja logige sisse OneDrive ' i.</span><span class="sxs-lookup"><span data-stu-id="4210a-113">Reboot the computer, and log into OneDrive.</span></span>