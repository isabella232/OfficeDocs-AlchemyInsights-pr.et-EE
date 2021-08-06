---
title: Käivita Windows mäludiagnostika Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 63ba3afdd8f74b17559484f37e9250587aec9b4a929325d8f82e3c9ad06f1783
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922537"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Käivita Windows mäludiagnostika Windows 10

Kui Windows ja teie arvutis olevad rakendused krahhi, külmutavad või käituvad ebastabiilselt, võib teil olla arvuti mäluga (RAM) probleeme. Saate käivitada Windows mäludiagnostika, et kontrollida arvuti muutmäluga seotud probleeme.

Tippige tegumiriba otsinguväljale mäludiagnostika ja seejärel valige Windows **Mäludiagnostika**.  

Diagnostika käivitamiseks peab arvuti taaskäivitama. Saate kohe taaskäivitada (salvestage oma töö ja sulgege esmalt avatud dokumendid ja meilisõnumid) või ajastada diagnostika automaatseks käivitamiseks järgmisel arvuti taaskäivitamisel.

![Windows Mäludiagnostika](media/windows-memory-diagnostic.png)

Arvuti taaskäivitamisel käivitub **Windows mäludiagnostika** tööriist automaatselt. Olek ja edenemine kuvatakse diagnostika käivitamiseks ning teil on võimalus diagnostika tühistada, kui vajutate **klaviatuuril paoklahvi (ESC).**

Kui diagnostika on lõpule viidud, Windows käivitub see tavapäraselt.
Kohe pärast taaskäivitamist kuvatakse töölaua kuvamisel teatis (tegumiribal tegevuskeskuse ikooni kõrval), mis näitab, kas mälutõrgei leiti.  Näide.

Tegevuskeskuse ikoon on järgmine. ![Tegevuskeskuse ikoon](media/action-center-icon.png) 

Ja näidisteatis: ![Mälutõrgeteta](media/no-memory-errors.png)

Kui te ei saanud teatist, saate tegevuskeskuse kuvamiseks  ja teatiste keritava loendi kuvamiseks valida tegumiribal tegevuskeskuse ikooni. 

Üksikasjaliku teabe läbivaatamiseks tippige **sündmus** tegumiriba otsinguväljale ja seejärel valige **Sündmusevaatur**. Liikuge **sündmusevaaturi** vasakpoolsel paanil lehele **Windows Logid > .** Otsige parempoolsel paanil loendit allapoole, vaadates veergu Allikas, **kuni** näete sündmusi, mille väärtus **on MemoryDiagnostics-Results**. Tõstke iga selline sündmus esile ja vaadake tulemiteavet loendi all **vahekaardi Üldist** väljal.
