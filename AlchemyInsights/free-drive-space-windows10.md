---
title: Windows 10 kõvakettaruumi vabastamine
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035667"
---
# <a name="free-up-drive-space-in-windows-10"></a>Windows 10 kõvakettaruumi vabastamine

Windowsi kettaruumi vabastamiseks on kaks võimalust.

- Vabastage Windows 10 kõvakettaruumi.
- Vabastage ruumi Windows 10 värskenduste jaoks välise mäluseadme abil.

Kui teil on pärast kettapuhastuse kasutamist endiselt väike kettaruum, on võimalik, et teie temp-kaust täidab kiiresti rakenduse (. appx) failid, mida Microsoft Store kasutab. Probleemi lahendamiseks lähtestage pood, tühjendage ruut Talleta vahemälu ja seejärel käivitage Windows Update ' i tõrkeotsija. Enne nende toimingute jätkamist veenduge, et Microsoft Store oleks suletud.

**1. juhis: Microsoft Store ' i lähtestamine**

**Märkus** See kustutab seadmest jäädavalt rakenduse andmed, sh teie eelistused ja sisselogimise üksikasjad.

1. Valige menüü **Start**  >  **sätted**  >  **rakendused**  >  **& funktsioonid**.

1. Otsige rakenduste loendist üles ja valige Microsoft Store.

1. Valige **Täpsemad suvandid**.

1. Kerige allapoole ja valige **Lähtesta** ja seejärel **kinnitage lähtestamine**.

**2. juhis: Microsoft Store ' i vahemälu tühjendamine**

1. Vajutage klahvikombinatsiooni Windowsi logoga klahv + R, et avada dialoogiboks Käivita.

1. Tippige wsreset.exe ja klõpsake **nuppu OK**.

1. Avaneb tühja käsuviiba aken. Umbes 10 sekundi pärast sulgub aken ja pood avaneb automaatselt.

**3. juhis: Windows Update ' i lähtestamine**

1. Valige käsk **Alusta**  >  **sätteid**  >  **Värskenda & turvalisuse**  >  **tõrkeotsing**.

1. Liikuge kerides allapoole ja valige loendist **Windows Update** ja valige käsk **Käivita tõrkeotsija**.

1. Taaskäivitage arvuti ja kontrollige, kas teil on endiselt probleeme.

