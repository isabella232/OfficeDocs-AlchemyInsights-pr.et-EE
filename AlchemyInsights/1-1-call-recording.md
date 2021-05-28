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
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696918"
---
# <a name="11-call-recording"></a><span data-ttu-id="5cb8b-102">1:1 kõne salvestamine</span><span class="sxs-lookup"><span data-stu-id="5cb8b-102">1:1 call recording</span></span>

<span data-ttu-id="5cb8b-103">Kui **nupp Alusta salvestamist** on 1:1 kõnes tuhm, peate muutma mõjutatud kasutaja poliitikasätteid.</span><span class="sxs-lookup"><span data-stu-id="5cb8b-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span>   

<span data-ttu-id="5cb8b-104">Alates 31. maist 2021 alustame uue kõnepoliitika Teams *AllowCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="5cb8b-104">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="5cb8b-105">Enne seda muudatust reguleerib 1:1 kõne salvestamist *AllowCloudRecording* Teams koosolekupoliitika.</span><span class="sxs-lookup"><span data-stu-id="5cb8b-105">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="5cb8b-106">See muudatus on dokumenteeritud sõnumikeskuse postituses: [(Värskendatud) 1:1 Kõnesalvestuspoliitika tutvustus.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)</span><span class="sxs-lookup"><span data-stu-id="5cb8b-106">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="5cb8b-107">*AllowCloudRecordingForCalls*   helistamispoliitika suvand on **$False** vaikimisi määratud.</span><span class="sxs-lookup"><span data-stu-id="5cb8b-107">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="5cb8b-108">Kui eelistate blokeerida kõigi kasutajate 1:1 kõnede salvestamise, ei pea te midagi tegema.</span><span class="sxs-lookup"><span data-stu-id="5cb8b-108">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="5cb8b-109">Kõne salvestamise lubamiseks kõigile kasutajatele 1:1 kõnes kasutage powerShelli Teams käivitamiseks järgmist cmdlet-käsku.</span><span class="sxs-lookup"><span data-stu-id="5cb8b-109">To enable call recording for all users in 1:1 calls use Teams PowerShell to run the following cmdlet:</span></span> 

<span data-ttu-id="5cb8b-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="5cb8b-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="5cb8b-111">Teise võimalusena saate luua uue poliitika ja määrata **-AllowCloudRecordingForCalls** **$true** ja määrata selle poliitika oma kasutajatele.</span><span class="sxs-lookup"><span data-stu-id="5cb8b-111">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="5cb8b-112">Lisateavet leiate teemast [1:1 Kõnesalvestuspoliitika juhtelemendid on (peaaegu!) Siin](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span><span class="sxs-lookup"><span data-stu-id="5cb8b-112">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
