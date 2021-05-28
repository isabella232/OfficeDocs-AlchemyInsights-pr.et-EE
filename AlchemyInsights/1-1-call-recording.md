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
# <a name="11-call-recording"></a>1:1 kõne salvestamine

Kui **nupp Alusta salvestamist** on 1:1 kõnes tuhm, peate muutma mõjutatud kasutaja poliitikasätteid.   

Alates 31. maist 2021 alustame uue kõnepoliitika Teams *AllowCloudRecordingForCalls*. Enne seda muudatust reguleerib 1:1 kõne salvestamist *AllowCloudRecording* Teams koosolekupoliitika. See muudatus on dokumenteeritud sõnumikeskuse postituses: [(Värskendatud) 1:1 Kõnesalvestuspoliitika tutvustus.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)  

*AllowCloudRecordingForCalls*   helistamispoliitika suvand on **$False** vaikimisi määratud. Kui eelistate blokeerida kõigi kasutajate 1:1 kõnede salvestamise, ei pea te midagi tegema.  

Kõne salvestamise lubamiseks kõigile kasutajatele 1:1 kõnes kasutage powerShelli Teams käivitamiseks järgmist cmdlet-käsku. 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Teise võimalusena saate luua uue poliitika ja määrata **-AllowCloudRecordingForCalls** **$true** ja määrata selle poliitika oma kasutajatele. 

Lisateavet leiate teemast [1:1 Kõnesalvestuspoliitika juhtelemendid on (peaaegu!) Siin](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
