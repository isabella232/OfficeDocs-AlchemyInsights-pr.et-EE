---
title: Näidikud ei tööta Edge'i brauseris
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676239"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Näidikud ei tööta Edge'i brauseris

Pärast näidiku loomist ei pea Edge (Smartscreen) seda austama. Lisateavet leiate teemast [IPde ja URL-ide/domeenide näidikute loomine.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)

## <a name="step-1-ensure-the-following"></a>1. juhis. Veenduge, et

- Veenduge, et indikaator on õige (IP/URL-is ei ole kirjavigu, õige toiming, õiged RBAC-rühmad).
- Võimaliku latentsuse arvesse miseks oodake pärast näidiku loomist vähemalt 2 tundi.
- Veenduge, et süsteem(id) on microsoft Defenderi lõpp-punkti jaoks sisse logitud.
- Veenduge, et süsteem(id) saaks pilveteenusega suhelda.
- Kontrollige, kas Smartscreen on lubatud ja kasutatav, kui avate [testimissaidi.](https://demo.smartscreen.msft.net)

## <a name="step-2-troubleshoot-the-potential-issue"></a>2. juhis. Võimaliku probleemi tõrkeotsing

- Veenduge, et klient vastaks nõuetele. Lisateavet leiate teemast [IPde ja URL-ide/domeenide jaoks näidikute loomine.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)
- Veenduge, et kasutate Edge'i brauseri uusimat versiooni. Uusima versiooni kohta leiate teavet teemast [Microsoft Edge versioon.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)
- Taaskäivitage Edge'i brauser.
- Liikuge saidile, mille jaoks olete näidiku häälestanud. Kui sait ei kuvata ootuspäraselt, jätkake 3. juhise kasutamist. 

## <a name="step-3-collect-data"></a>3. juhis: andmete kogumine

- Koguge **MDEClientAnalyzeri diagnostikaandmeid.** Juhised leiate teemast Microsoft Defender for Endpoint'ile [sisseldumisseadmetega seotud probleemid.](issues-with-onboarding-machines.md)
- Kui teil on mugav Fiddleri jälitust installida ja koguda, lugege [teemat Telerik Fiddler](http://www.telerik.com/fiddler).
- Kui eelistate Microsofti tugiteenuste juhiseid, valige tugiteenuse juhtumi avamiseks allpool ikoon Tugi.
