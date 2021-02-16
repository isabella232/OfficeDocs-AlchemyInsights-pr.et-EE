---
title: Seadme lubamine
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8278"
ms.openlocfilehash: 9e4b03dcba7a2c98a5d63213ee49f9ba8f91d670
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256759"
---
# <a name="enable-device"></a><span data-ttu-id="67e80-102">Seadme lubamine</span><span class="sxs-lookup"><span data-stu-id="67e80-102">Enable Device</span></span>

<span data-ttu-id="67e80-103">**Seadme lubamine PowerShelli käsu abil**</span><span class="sxs-lookup"><span data-stu-id="67e80-103">**To enable the device using Powershell command**</span></span>

<span data-ttu-id="67e80-104">Käivitage järgmised käsud.</span><span class="sxs-lookup"><span data-stu-id="67e80-104">Run the following commands:</span></span>

- <span data-ttu-id="67e80-105">Seadme objekti hankimiseks tehke järgmist. `Get-MsolDevice -Name <Name>`</span><span class="sxs-lookup"><span data-stu-id="67e80-105">To get device object: `Get-MsolDevice -Name <Name>`</span></span>
- <span data-ttu-id="67e80-106">Seadme lubamiseks tehke järgmist. `Enable-MsolDevice -DeviceId <DeviceId>`</span><span class="sxs-lookup"><span data-stu-id="67e80-106">To enable device: `Enable-MsolDevice -DeviceId <DeviceId>`</span></span>

<span data-ttu-id="67e80-107">Lisateavet hallatavate domeenide hübriidiga liitumise kohta leiate teemast [hübriidiga liitumise konfigureerimine](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains).</span><span class="sxs-lookup"><span data-stu-id="67e80-107">For more information on Configuring Hybrid Join on managed domains, see [Configure Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains).</span></span>
