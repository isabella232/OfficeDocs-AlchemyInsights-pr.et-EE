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
ms.openlocfilehash: 8cdadf34a059856338d7f40528446b70373465e4
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702086"
---
# <a name="11-call-recording"></a><span data-ttu-id="aadce-102">1:1 kõne salvestamine</span><span class="sxs-lookup"><span data-stu-id="aadce-102">1:1 call recording</span></span>

<span data-ttu-id="aadce-103">Kui **nupp Alusta salvestamist** on 1:1 kõnes tuhm, peate muutma mõjutatud kasutaja poliitikasätteid.</span><span class="sxs-lookup"><span data-stu-id="aadce-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span> <span data-ttu-id="aadce-104">Poliitikasätte määramiseks käivitage mõjutatud kasutaja jaoks diagnostika, tippides **diag: Teams 1:1 Kõne salvestamine.**</span><span class="sxs-lookup"><span data-stu-id="aadce-104">To check the policy setting, run the Diagnostic for the impacted user by typing **Diag: Teams 1:1 Call Recording** above.</span></span>     

<span data-ttu-id="aadce-105">Alates 31. maist 2021 alustame uue kõnepoliitika Teams *AllowCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="aadce-105">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="aadce-106">Enne seda muudatust reguleerib 1:1 kõne salvestamist *AllowCloudRecording* Teams koosolekupoliitika.</span><span class="sxs-lookup"><span data-stu-id="aadce-106">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="aadce-107">See muudatus on dokumenteeritud sõnumikeskuse postituses: [(Värskendatud) 1:1 Kõnesalvestuspoliitika tutvustus.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)</span><span class="sxs-lookup"><span data-stu-id="aadce-107">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="aadce-108">*AllowCloudRecordingForCalls*   helistamispoliitika suvand on **$False** vaikimisi määratud.</span><span class="sxs-lookup"><span data-stu-id="aadce-108">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="aadce-109">Kui eelistate blokeerida kõigi kasutajate 1:1 kõnede salvestamise, ei pea te midagi tegema.</span><span class="sxs-lookup"><span data-stu-id="aadce-109">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="aadce-110">Kõne salvestamise lubamiseks kõigile kasutajatele 1:1 kõnes [kasutage powerShelli Teams käivitamiseks](/microsoftteams/teams-powershell-install) järgmist cmdlet-käsku.</span><span class="sxs-lookup"><span data-stu-id="aadce-110">To enable call recording for all users in 1:1 calls use [Teams PowerShell](/microsoftteams/teams-powershell-install) to run the following cmdlet:</span></span> 

<span data-ttu-id="aadce-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="aadce-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="aadce-112">Teise võimalusena saate luua uue poliitika ja määrata **-AllowCloudRecordingForCalls** **$true** ja määrata selle poliitika oma kasutajatele.</span><span class="sxs-lookup"><span data-stu-id="aadce-112">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="aadce-113">Lisateavet leiate teemast [1:1 Kõnesalvestuspoliitika juhtelemendid on (peaaegu!) Siin](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span><span class="sxs-lookup"><span data-stu-id="aadce-113">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
