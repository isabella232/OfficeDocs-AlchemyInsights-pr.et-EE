---
title: Microsoft Edge'i täiustatud autentimispõhimõtted
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398554"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Microsoft Edge'i täiustatud autentimispõhimõtted

Microsoft Edge'ile kehtivad täpsemad autentimismõisted on järgmised.

**Ennetav autentimine**

Kui lubate [poliitika ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) proovib Microsoft Edge ennetavalt autentida sisse logitud kasutajaid Microsofti teenuste kaudu. Regulaarsete intervallide järel kontrollib see veebiteenuse abil värskendatud manifesti, mis sisaldab proaktiivset autentimist reguleerivat konfiguratsiooni.

Eelised. Ennetav autentimine võimaldab autentimist võtmeteenustele (nt Office'i uue vahekaardi lehele). Kui Bingi kasutatakse otsingumootorina, parandab proaktiivne autentimine aadressiriba jõudlust ja aitab luua teie ettevõtte vajadustele kohandatud otsingutulemeid.

**Windows Hello CredUI NTLM-autentimise jaoks**

Kui ühekordne sisselogimine (SSO) pole saadaval, kui veebisait proovib kasutajat NTLM-i või Negotiatei mehhanismi kaudu sisse logida, võimaldab see funktsioon kasutajal operatsioonisüsteemi identimisteavet veebisaidiga jagada ja windows Hello Credi kasutajaliidese abil autentimisfunktsiooni abil rahuldada. See sisselogimisvoog kuvatakse ainult opsüsteemis Windows 10 ja ainult kasutajatele, kes ei saa SSO-d NTLM-i või Negotiatei väljakutse ajal.

**Salvestatud paroolide kasutamine automaatseks sisselogimiseks**

Microsoft Edge'is paroole salvestavad kasutajad saavad lubada automaatse sisselogimise veebisaitidele, kus nad on identimisteabe salvestanud. Kasutajad saavad selle funktsiooni sisse või välja edge://settings/passwords ja saate selle konfigureerida [paroolihalduri poliitikates.](https://go.microsoft.com/fwlink/?linkid=2134622)
