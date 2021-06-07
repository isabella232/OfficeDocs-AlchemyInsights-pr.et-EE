---
title: Veebisenaride registreerimise haldamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793709"
---
# <a name="manage-webinar-registration"></a>Veebisenaride registreerimise haldamine

PowerShelli käskude abil saate Teams veebiportaalide Teams kasutajaks registreeruda. PowerShelli Teams leiate teemast [Teams PowerShell](/microsoftteams/teams-powershell-install). 

Vaikimisi on *WhoCanRegister* lubatud ja selle väärtuseks on seatud **EveryoneInCompany**. Selleks et lubada kõigil (sh anonüümsetel kasutajatel) registreeruda, peate powershelli käsu abil määrama koosolekupoliitika väärtuseks Kõik. 

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Märkus.** Kui anonüümne liitumine on koosolekusätetes välja lülitatud, ei saa anonüümsed kasutajad veebiseinaritega liituda. Lisateavet ja selle sätte lubamise kohta leiate teemast [Koosolekusätete haldamine Microsoft Teams](/microsoftteams/meeting-settings-in-teams).

Kui soovite koosoleku registreerimise välja lülitada, määrake *allowMeetingRegistration väärtuseks* **False (Väär).**

Lisateavet selle kohta, kes saab veebiseinarite jaoks registreeruda, leiate teemast [Webinarsi kasutajaks registreerujate konfigureerimine.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) Lisateavet Microsofti loendite sätete kohta leiate teemast [Microsofti loendite sätete juhtimine.](/sharepoint/control-lists)
