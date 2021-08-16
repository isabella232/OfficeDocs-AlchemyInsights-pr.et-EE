---
title: Microsoft Defenderi täiustatud ohutõrje Windows 10 kaugjuurdepääsu probleemide lahendamine
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 44969436c99b182cb4202fa60e2deb7d6ea3f460e48ee4649de1cfb646970f34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034030"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Microsoft Defenderi täiustatud ohutõrje Windows 10 kaugjuurdepääsu probleemide lahendamine

Kui pääsete juurde kaugarvutile, tehke järgmist.

1. Laadige alla [klientrakenduse ühenduvuse analüsaatori](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostikatööriist.
2. Ekstraktige ja käivitage MDATPAnalyzer.cmd.
3. Otsige diagnostikalogi üles kaustast MDATPClientAnalyzerResult, mis on sama kaust, kuhu analüsaatori tööriist alla laaditi.
4. Ühenduvuse või Interneti-puhverserveri sätetega seotud probleemide leidmiseks vaadake logifaili MDATPClientAnalyzer.txt.

Lisateavet leiate teemast [Probleemid pardaseadmetega.](https://go.microsoft.com/fwlink/?linkid=2143634)
