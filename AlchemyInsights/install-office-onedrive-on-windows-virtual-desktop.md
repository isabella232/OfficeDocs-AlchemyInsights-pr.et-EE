---
title: Office'i ja OneDrive'i installimine Windows Virtual Desktopi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595624"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a><span data-ttu-id="e4b86-102">Office'i ja OneDrive'i installimine Windows Virtual Desktopi</span><span class="sxs-lookup"><span data-stu-id="e4b86-102">Install Office and OneDrive on Windows Virtual Desktop</span></span>

1. <span data-ttu-id="e4b86-103">[Valmistage ette ja kohandage juht-VHD-pilti.](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image)</span><span class="sxs-lookup"><span data-stu-id="e4b86-103">[Prepare and customize a master VHD image](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image).</span></span> <span data-ttu-id="e4b86-104">Looge virtuaalarvuti (VM), kui seda pole veel loodud.</span><span class="sxs-lookup"><span data-stu-id="e4b86-104">Create a virtual machine (VM) if it hasn't already been created.</span></span>

1. <span data-ttu-id="e4b86-105">[Installige Office ühisarvuti aktiveerimisrežiimis.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode)</span><span class="sxs-lookup"><span data-stu-id="e4b86-105">[Install Office in shared computer activation mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode).</span></span> <span data-ttu-id="e4b86-106">Ühisarvuti aktiveerimine võimaldab mitmel kasutajal Office'ile juurde pääseda.</span><span class="sxs-lookup"><span data-stu-id="e4b86-106">Shared computer activation allows multiple users to access Office.</span></span>

1. <span data-ttu-id="e4b86-107">[Installige OneDrive seadme kohta.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode)</span><span class="sxs-lookup"><span data-stu-id="e4b86-107">[Install OneDrive in per-machine mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode).</span></span> <span data-ttu-id="e4b86-108">Tavaliselt installitakse OneDrive kasutaja kohta, kuid siin peaks see olema installitud seadme kohta.</span><span class="sxs-lookup"><span data-stu-id="e4b86-108">Normally, OneDrive is installed per user, but here, it should be installed per machine.</span></span>