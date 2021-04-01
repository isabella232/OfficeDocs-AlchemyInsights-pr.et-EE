---
title: Microsoft Edge'i seadis macOS-seadme vaikebrauseriks
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491426"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="34856-102">Microsoft Edge'i seadis macOS-seadme vaikebrauseriks</span><span class="sxs-lookup"><span data-stu-id="34856-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="34856-103">Microsoft Edge'i vaikebrauseriks vaatamiseks kasutage ühte kahest meetodist.</span><span class="sxs-lookup"><span data-stu-id="34856-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="34856-104">1. meetod. Seadme vilkumine macOS-i pildiga, kus Microsoft Edge on juba vaikebrauseriks määratud.</span><span class="sxs-lookup"><span data-stu-id="34856-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="34856-105">2. meetod. Määrake poliitika DefaultBrowserSettingEnabled ( VaikebrowserSettingEnabled), et paluda kasutajal seada Microsoft Edge vaikebrauseriks.</span><span class="sxs-lookup"><span data-stu-id="34856-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="34856-106">Kumbki meetod võimaldab kasutajal vaikebrauseri muuta.</span><span class="sxs-lookup"><span data-stu-id="34856-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="34856-107">Seetõttu soovitame juurutada poliitika DefaultBrowserSettingEnabled isegi siis, kui kasutasite meetodit 1.</span><span class="sxs-lookup"><span data-stu-id="34856-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="34856-108">Kui kasutaja muudab pärast poliitika juurutamist vaikebrauseri, palub poliitika kasutajal seada vaikebrauseriks tagasi Microsoft Edge'i.</span><span class="sxs-lookup"><span data-stu-id="34856-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
