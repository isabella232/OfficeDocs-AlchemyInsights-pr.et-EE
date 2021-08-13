---
title: Windows 10 kettaruumi vabastamine
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
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: c7d29ab718be8dbdcde61a7de2f158fb3bbd722d2964d8b13cde9936dd1e5ee1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53928077"
---
# <a name="free-up-drive-space-in-windows-10"></a>Windows 10 kettaruumi vabastamine

Siit leiate Windowsis kettaruumi vabastamiseks kaks võimalust.

- Vabastage Windows 10 kettaruumi.
- Vabastage Windows 10 värskenduste jaoks kettaruumi välise mäluseadme abil.

Kui pärast kettapuhastust on kettaruumi endiselt vähe, võib probleem olla selles, et ajutiste failide kaust Temp täidetakse kiiresti Microsoft Store’i kasutatavate rakendusefailidega (.appx). Probleemi lahendamiseks lähtestage Microsoft Store, tühjendage Microsoft Store’i vahemälu ja seejärel käivitage Windows Update’i tõrkeotsing. Enne järgmiste toimingute tegemist tuleb Microsoft Store kindlasti sulgeda.

**1. toiming: Microsoft Store’i lähtestamine**

**Märkus** See kustutab seadmest jäädavalt rakenduseandmed (sh eelistused ja sisselogimisandmed).

1. Valige **Start** > **Sätted** > **Rakendused** > **Rakendused ja funktsioonid**.

1. Otsige rakenduste loendist üles Microsoft Store ja valige see.

1. Valige **Täpsemad suvandid**.

1. Kerige allapoole ja valige **Lähtesta** ja seejärel **kinnitage lähtestamine**.

**2. toiming: Microsoft Store’i vahemälu tühjendamine**

1. Dialoogiboksi „Käivita“ avamiseks vajutage klahvikombinatsiooni Windowsi logoga klahv + R.

1. Tippige wsreset.exe ja valige **OK**.

1. Avaneb tühi käsuviibaaken. Umbes 10 sekundi pärast sulgub aken automaatselt ja avaneb Microsoft Store.

**3. toiming: Windows Update’i lähtestamine**

1. Valige **Start** > **Sätted** > **Värskendamine ja turvalisus** > **Tõrkeotsing**.

1. Kerige allapoole ja valige loendist **Windows Update** ning valige **Käivita tõrkeotsing**.

1. Taaskäivitage arvuti ja kontrollige, kas probleem on lahendatud.

