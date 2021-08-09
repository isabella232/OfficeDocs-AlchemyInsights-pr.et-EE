---
title: Täiustatud autentimismõisted, mida Microsoft Edge
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
ms.openlocfilehash: 8ddec37260ec4e3bcc390dcc8adb7397368de19555ee31be458be033d3886386
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934361"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Täiustatud autentimismõisted, mida Microsoft Edge

Järgmised on täiustatud autentimismõisted, mis kehtivad Microsoft Edge.

**Ennetav autentimine**

Kui lubate [poliitika ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge proovib kasutajaid ennetavalt autentida Microsofti teenused. Regulaarsete intervallide järel kontrollib see veebiteenuse abil värskendatud manifesti, mis sisaldab proaktiivset autentimist reguleerivat konfiguratsiooni.

Eelised. Ennetav autentimine võimaldab autentimist peamistele teenustele (nt Office menüülehele). Kui Bing kasutatakse otsingumootorina, parandab proaktiivne autentimine aadressiriba jõudlust ja aitab luua teie ettevõtte vajadustele kohandatud otsingutulemeid.

**Windows Hello CREDUI NTLM-autentimise jaoks**

Kui ühekordne sisselogimine (SSO) pole saadaval, kui veebisait proovib kasutajat NTLM-i või Negotiatei mehhanismi kaudu sisse logida, võimaldab see funktsioon kasutajal jagada os-i identimisteavet veebisaidiga ja Windows Hello Credi kasutajaliidese abil. See sisselogimisvoog kuvatakse ainult Windows 10 kasutajatele, kes ei saa SSO-d NTLM-i või Negotiatei väljakutse ajal.

**Salvestatud paroolide kasutamine automaatseks sisselogimiseks**

Kasutajad, kes salvestavad paroole Microsoft Edge saavad lubada automaatse sisselogimise veebisaitidele, kus nad on identimisteabe salvestanud. Kasutajad saavad selle funktsiooni sisse või välja edge://settings/passwords ja saate selle konfigureerida [paroolihalduri poliitikates.](https://go.microsoft.com/fwlink/?linkid=2134622)
