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
# <a name="11-call-recording"></a>1:1 kõne salvestamine

Administraatorid peavad nüüd võtma meetmeid, et lubada kasutajatel 1:1 kõnede salvestamist.
 
Algab 12 aprill, 2021, alustame uute Teamsi kõnede poliitika *AllowCloudRecordingForCalls*. 

Praegu on 1:1 kõnede salvestamise võimalused *AllowCloudRecording* töörühma koosoleku poliitikates. Kui teie kasutajatel on lubatud salvestada töörühma koosolekuid, saavad nad ka 1:1 kõnesid salvestada.

Kui soovite blokeerida kõik kasutajad 1:1 kõnede salvestamise eest, pole teil vaja midagi teha. *AllowCloudRecordingForCalls* kõnede poliitika suvand on vaikimisi $FALSE.

See muudatus on dokumenteeritud järgmises sõnumikeskuse postituses: [(värskendatud) 1:1 kõne salvestamise poliitika tutvustus](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) töörühma kõnede poliitika määramiseks peate kasutama [teamsi PowerShelli](https://docs.microsoft.com/microsoftteams/teams-powershell-install).

Kõnede **salvestamise lubamiseks 1:1 kõnesid:** Set-CsTeamsCallingPolicy-Identity Global-AllowCloudRecordingForCalls $True

Kõnede **salvestamise keelamiseks 1:1 kõnesid:** Set-CsTeamsCallingPolicy-identiteedi globaalse-AllowCloudRecordingForCalls $FALSE

