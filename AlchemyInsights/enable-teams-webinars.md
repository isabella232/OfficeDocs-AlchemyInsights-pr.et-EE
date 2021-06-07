---
title: Luba Teams webinars
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793651"
---
# <a name="enable-teams-webinars"></a>Luba Teams webinars

Webinars on vaikimisi lubatud. PowerShelli käskude abil saate hallata, kes Teams ajastada ja Teams veebipõhiseid Teams registreerida.

- Kõik kasutajad, kes saavad koosolekut luua, saavad luua ka veebisenarkoosoleku. Kui soovite hallata seda, kes saab Teams ajastada, kasutage funktsiooni *AllowMeetingRegistration*. 
- Vaikimisi on *WhoCanRegister* lubatud ja selle väärtuseks on **seatud Kõik**. Kui soovite koosoleku registreerimise välja lülitada, määrake *allowMeetingRegistration väärtuseks* **False (Väär).**

Nende sätete muutmiseks peate installima [Teams PowerShelli.](/microsoftteams/teams-powershell-install) Lisaks jõustatakse koosolekupoliitikad Teams webinars. Näiteks kui anonüümne liitumine on koosolekusätetes välja lülitatud, ei saa anonüümsed kasutajad veebiseinaritega liituda.

Lisateavet selle kohta, kes saab veebiseinarite jaoks registreeruda, leiate teemast [Webinarsi kasutajaks registreerujate konfigureerimine.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) Lisateavet Microsofti loendite sätete kohta leiate teemast [Microsofti loendite sätete juhtimine.](/sharepoint/control-lists)