---
title: 1:1 kõne salvestamine
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733845"
---
# <a name="11-call-recording"></a><span data-ttu-id="ce7ee-102">1:1 kõne salvestamine</span><span class="sxs-lookup"><span data-stu-id="ce7ee-102">1:1 call recording</span></span>

<span data-ttu-id="ce7ee-103">Administraatorid peavad nüüd võtma meetmeid, et lubada kasutajatel 1:1 kõnede salvestamist.</span><span class="sxs-lookup"><span data-stu-id="ce7ee-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="ce7ee-104">Algab 12 aprill, 2021, alustame uute Teamsi kõnede poliitika *AllowCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="ce7ee-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="ce7ee-105">Praegu on 1:1 kõnede salvestamise võimalused *AllowCloudRecording* töörühma koosoleku poliitikates.</span><span class="sxs-lookup"><span data-stu-id="ce7ee-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="ce7ee-106">Kui teie kasutajatel on lubatud salvestada töörühma koosolekuid, saavad nad ka 1:1 kõnesid salvestada.</span><span class="sxs-lookup"><span data-stu-id="ce7ee-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="ce7ee-107">Kui soovite blokeerida kõik kasutajad 1:1 kõnede salvestamise eest, pole teil vaja midagi teha.</span><span class="sxs-lookup"><span data-stu-id="ce7ee-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="ce7ee-108">*AllowCloudRecordingForCalls* kõnede poliitika suvand on vaikimisi $FALSE.</span><span class="sxs-lookup"><span data-stu-id="ce7ee-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="ce7ee-109">See muudatus on dokumenteeritud järgmises sõnumikeskuse postituses: [(värskendatud) 1:1 kõne salvestamise poliitika tutvustus](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) töörühma kõnede poliitika määramiseks peate kasutama [teamsi PowerShelli](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="ce7ee-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="ce7ee-110">Kõnede **salvestamise lubamiseks 1:1 kõnesid:** Set-CsTeamsCallingPolicy-Identity Global-AllowCloudRecordingForCalls $True</span><span class="sxs-lookup"><span data-stu-id="ce7ee-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="ce7ee-111">Kõnede **salvestamise keelamiseks 1:1 kõnesid:** Set-CsTeamsCallingPolicy-identiteedi globaalse-AllowCloudRecordingForCalls $FALSE</span><span class="sxs-lookup"><span data-stu-id="ce7ee-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

