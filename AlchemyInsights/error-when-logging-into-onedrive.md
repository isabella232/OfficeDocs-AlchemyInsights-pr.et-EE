---
title: 0x8004de40 OneDrive'i käivitamisel ilmnes tõrge
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813648"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="0a270-102">0x8004de40 OneDrive'i käivitamisel ilmnes tõrge</span><span class="sxs-lookup"><span data-stu-id="0a270-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="0a270-103">Kui **OneDrive'0x8004de40** sisselogimisel kuvatakse tõrketeade, taaskäivitage arvuti töö- või koolidomeeniga ühenduse loomise ajal.</span><span class="sxs-lookup"><span data-stu-id="0a270-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="0a270-104">Kui teile kuvatakse see tõrge pärast taaskäivitamist, proovige seda töö- või koolidomeeniga ühenduse saamisel.</span><span class="sxs-lookup"><span data-stu-id="0a270-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="0a270-105">Klõpsake nuppu Start ja  tippige **otsinguväljale tekst cmd** või käsuviip, paremklõpsake käsuviiba rakendust ja valige **Käivita administraatorina**.</span><span class="sxs-lookup"><span data-stu-id="0a270-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="0a270-106">Kui teilt küsitakse administraatoriparooli või kinnitust, tippige parool või klõpsake nuppu **Luba**.</span><span class="sxs-lookup"><span data-stu-id="0a270-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="0a270-107">Tippige aknas Käsuviip **tekst dsregcmd /leave**  ja oodake, kuni käsk lõpule jõuaks.</span><span class="sxs-lookup"><span data-stu-id="0a270-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="0a270-108">Seejärel tippige **dsregcmd /join** ja oodake, kuni käsk on lõpule viidud.</span><span class="sxs-lookup"><span data-stu-id="0a270-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="0a270-109">Taaskäivitage arvuti.</span><span class="sxs-lookup"><span data-stu-id="0a270-109">Reboot your computer.</span></span>
