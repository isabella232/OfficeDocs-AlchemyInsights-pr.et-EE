---
title: Teams ei käivitu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/4/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12673"
- "9007646"
ms.openlocfilehash: a37f980e700090da8199c703216af6f04f4aca464c21870beb3e907dd7b2d491
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813345"
---
# <a name="teams-doesnt-launch"></a>Teams ei käivitu

Kui proovite faili avada Microsoft Teams kuid see ei käivitu kunagi, proovige järgmist.

1. Liikuge **sirvides asukohta %appdata%\Microsoft\Teams**.
1. Kustutage kausta sisu.
1. Taaskäivitage arvuti ja proovige käivitada Teams.

Võimalik, et peate selle uuesti Teams. Uuesti installimiseks:

1. Desinstallige Teams juhtpaneeli abil.
1. Liikuge **sirvides asukohta %appdata%\Microsoft\Teams\Application Cache**.
1. Kustutage kausta sisu.
1. Liikuge **sirvides asukohta %appdata%\Microsoft\teams\Cache**.
1. Kustutage kausta sisu.
1. Taaskäivitage arvuti ja seejärel laadige alla ja installige Teams.

Kui soovite rentnikus käivitada diagnostika kindla kasutaja jaoks, kes ei saa sisse logida, käivitage uus otsing **märksõnaga TeamsUserUnableToSignIn** ja järgige viipasid.