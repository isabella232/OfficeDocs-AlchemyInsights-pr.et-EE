---
title: Probleemide lahendamine Windows 10 seadmetes Microsoft Defenderi täiustatud ohtude kaitsega
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
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693007"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Probleemide lahendamine Windows 10 seadmetes Microsoft Defenderi täiustatud ohtude kaitsega

Kui teil on juurdepääs kaugarvutiga, tehke järgmist.

1. Laadige alla [klientarvuti ühenduvuse analüsaatori](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostiline tööriist.
2. Ekstraktige ja käivitage MDATPAnalyzer. cmd.
3. Otsige üles kaust MDATPClientAnalyzerResult, mis on sama kaust, kus analüsaatori tööriist alla laaditi.
4. Kui soovite otsida probleeme ühenduvuse või Interneti-puhverserveri sätetega, vaadake logifaili MDATPClientAnalyzer.txt.

Lisateavet leiate teemast [masinate pardal](https://go.microsoft.com/fwlink/?linkid=2143634)olevad probleemid.
