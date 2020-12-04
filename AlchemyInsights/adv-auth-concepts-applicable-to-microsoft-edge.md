---
title: Microsoft Edge ' i suhtes kohaldatavad täiustatud autentimise põhimõtted
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
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573394"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Microsoft Edge ' i suhtes kohaldatavad täiustatud autentimise põhimõtted

Järgmised on Microsoft Edge ' i jaoks kohaldatavad täiustatud autentimise kontseptsioonid.

**Proaktiivne autentimine**

Kui lubate [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) poliitika, proovib Microsoft Edge autentida sisselogitud kasutajaid Microsofti teenuste kaudu. Regulaarsete ajavahemike järel kasutab ta veebiteenust, et kontrollida värskendatud manifesti, mis sisaldab ennetavat autentimist reguleerivat konfiguratsiooni.

Eelised: proaktiivne autentimine võimaldab autentida põhiteenuseid (nt Office ' i uue vahekaardi leht). Kui otsingumootorina kasutatakse ka Bingi, parandab proaktiivne autentimine aadressiriba jõudlust ja aitab luua teie ärirakenduse vajadustele vastavaid otsingutulemusi.

**Windows Hello CredUI NTLM-autentimise jaoks**

Kui üksik sisselogimine (SSO) pole saadaval, kui veebisait proovib sisse logida kasutaja kaudu NTLM-või läbirääkimiste mehhanismi kaudu, võimaldab see funktsioon kasutajal jagada selle saidiga OS-i mandaati ja rahuldada autentimise väljakutse Windows Hello-i-süsteemi KASUTAJALIIDESE abil. See sisselogimine kuvatakse ainult opsüsteemis Windows 10 ja ainult nende kasutajate jaoks, kes ei saa kasutada SSO-või läbirääkimiste väljakutset.

**Automaatselt sisselogimiseks salvestatud paroolide kasutamine**

Microsoft Edge ' is paroolid salvestavad kasutajad saavad lubada automaatse sisselogimise veebisaitidele, kus nad on salvestanud mandaadi. Kasutajad saavad selle funktsiooni edge://settings/passwords sisse või välja lülitada ja seda saab konfigureerida [parooli halduri](https://go.microsoft.com/fwlink/?linkid=2134622) poliitikas.
