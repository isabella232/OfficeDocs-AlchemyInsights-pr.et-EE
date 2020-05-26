---
title: Windowsi mäludiagnostika käivitamine Windows 10-s
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357515"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Windowsi mäludiagnostika käivitamine Windows 10-s

Kui arvuti Windows ja rakendused on krahh, külmutamine või ebastabiilsel viisil tegutsemine, võib teil olla probleem arvuti mäluga (RAM). ARVUTI RAM-i probleemide kontrollimiseks saate käivitada Windowsi mäludiagnostika.

Tippige tegumiriba otsinguväljale tekst **mälu diagnostika**ja seejärel valige **Windowsi mäludiagnostika**. 

Diagnostika käivitamiseks peab arvuti taaskäivitama. Teil on võimalus kohe taaskäivitada (salvestage oma töö ja sulgege avatud dokumendid ja e-kirjad kõigepealt) või ajastada diagnostika automaatseks käivitamiseks järgmine kord, kui arvuti taaskäivitub:

![Windowsi mäludiagnostika](media/windows-memory-diagnostic.png)

Kui arvuti taaskäivitub, käivitub **Windowsi mälutuvastustööriist** automaatselt. Olek ja edenemine kuvatakse diagnostika käivitada, ja teil on võimalus tühistada diagnostika lööb **ESC** klahvi klaviatuuril.

Kui diagnostika on lõpule jõudnud, hakkab Windows normaalselt käivituma.
Kohe pärast taaskäivitamist, kui kuvatakse töölaua, kuvatakse teade (kõrval tegumiribal **tegevuskeskuse** ikoon), et näidata, kas mälu tõrked leiti. Näiteks.

Siin on tegevuskeskuse ikoon: ![Tegevuskeskuse ikoon](media/action-center-icon.png) 

Ja näidisteatis: ![Mälu tõrkeid pole](media/no-memory-errors.png)

Kui teate vastamata, saate **tegevuskeskuse** kuvamiseks valida tegumiribal **tegevuskeskuse** ikooni ja vaadata teatiste keritav loend.

Üksikasjaliku teabe läbivaatamiseks tippige **sündmus** tegumiriba otsinguväljale ja seejärel valige **Sündmusevaatur**. Liikuge **sündmusevaaturi**vasakpoolsel paanil **Windowsi logid > System**. Skannige parempoolsel paanil loendit, vaadates veergu **Allikas** , kuni näete sündmusi, millel on allika väärtuse **memorydiagnostics-tulemused**. Tõstke iga selline sündmus esile ja vaadake tulemuste teavet kasti all vahekaardi **Üldine** loendis.
