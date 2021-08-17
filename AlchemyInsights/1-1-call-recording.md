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
ms.openlocfilehash: c17408442cec6c0877b7d66bc8a7fd3062eb0e47
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314380"
---
# <a name="11-call-recording"></a>1:1 kõne salvestamine

Kui **nupp Käivita salvestamine** on 1:1 kõnes tuhm, peate muutma mõjutatud kasutaja poliitikasätteid. Poliitikasätte määramiseks käivitage mõjutatud kasutaja jaoks diagnostika, tippides **diag: Teams 1:1 Kõne salvestamine.**     

Alates 31. maist 2021 alustame uue kõnepoliitika Teams *AllowCloudRecordingForCalls*. Enne seda muudatust kontrollib 1:1 kõne salvestamist *AllowCloudRecording* Teams koosolekupoliitika. See muudatus on dokumenteeritud sõnumikeskuse postituses: [(Värskendatud) 1:1 Kõnesalvestuspoliitika tutvustus.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)  

*AllowCloudRecordingForCalls*   helistamispoliitika suvand on **$False** vaikimisi määratud. Kui eelistate blokeerida kõigi kasutajate 1:1 kõnede salvestamise, ei pea te midagi tegema.  

Kõne salvestamise lubamiseks kõigile kasutajatele 1:1 kõnes [kasutage powerShelli Teams käivitamiseks](https://docs.microsoft.com/microsoftteams/teams-powershell-install) järgmist cmdlet-käsku. 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Teise võimalusena saate luua uue poliitika ja määrata **-AllowCloudRecordingForCalls** **$true** ja määrata selle poliitika oma kasutajatele. 

Lisateavet leiate teemast [1:1 Kõnesalvestuspoliitika juhtelemendid on (peaaegu!) Siin](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
