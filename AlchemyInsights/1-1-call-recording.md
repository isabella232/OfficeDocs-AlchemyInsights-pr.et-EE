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
ms.openlocfilehash: 29383643e6867bca7fd31774a9594b82fdc080bb0e7254141e8c883ad861075e
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57886135"
---
# <a name="11-call-recording"></a>1:1 kõne salvestamine

Kui **nupp Käivita salvestamine** on 1:1 kõnes tuhm, peate muutma mõjutatud kasutaja poliitikasätteid. Poliitikasätte määramiseks käivitage mõjutab kasutaja diagnostika, tippides **Diag: Teams 1:1 Kõne salvestamine** eespool.     

Alates 31. maist 2021 alustame uue kõnepoliitika Teams *AllowCloudRecordingForCalls*. Enne seda muudatust kontrollib 1:1 kõne salvestamist *AllowCloudRecording* Teams koosolekupoliitika. See muudatus on dokumenteeritud sõnumikeskuse postituses: [(Värskendatud) 1:1 Kõnesalvestuspoliitika tutvustus.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)  

*AllowCloudRecordingForCalls*   helistamispoliitika suvand on **$False** vaikimisi määratud. Kui eelistate blokeerida kõigi kasutajate 1:1 kõnede salvestamise, ei pea te midagi tegema.  

Kõnesalvestuse lubamiseks kõigile kasutajatele 1:1 kõnes [kasutage powerShelli Teams käivitamiseks](https://docs.microsoft.com/microsoftteams/teams-powershell-install) järgmist cmdlet-käsku. 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Teise võimalusena saate luua uue poliitika ja määrata **-AllowCloudRecordingForCalls** **$true** ja määrata selle poliitika oma kasutajatele. 

Lisateavet leiate teemast [1:1 Kõnesalvestuspoliitika juhtelemendid on (peaaegu!) Siin](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
