---
title: Ühenduspoliitika parandus
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
ms.openlocfilehash: 9094dcdc4507f52da1dd7c95f83aa98bab1446639d2d9f52eb3a7bc849dc183c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57888402"
---
# <a name="fix-connection-policy"></a>Ühenduspoliitika parandus

Meilisõnum oli märgitud turvaliseks ja toimetati kasutaja sisendkausta, kuna lähte-IP-aadress oli vaikeühendusfiltri poliitikas märgitud turvaliseks. Poliitika läbivaatamiseks tehke järgmist.

1. Avage Microsoft 365 Defender portaal jaotises Poliitikad <https://security.microsoft.com/> **& Meilipoliitikad** & Reeglid ohupoliitikad \>  \>  \>  Rämpspostitõrje. 

   Otse rämpspostitõrje **poliitikate lehele minemiseks** kasutage funktsiooni <https://security.microsoft.com/antispam> .

2. Valige **lehel Rämpspostitõrje poliitikad** poliitika nimega **Ühendusefiltri poliitika (vaikesäte),** klõpsates poliitika nime.

3. Klõpsake kuvatavas üksikasja hüpikmenüüs jaotises **Ühenduse filtreerimine** nuppu Redigeeri **ühendusfiltri** poliitikat.

4. Vaadake üle kirjed jaotises Luba **alati** järgmiste IP-aadresside või aadresside vahemiku sõnumid ja vaadake, **kas valitud on loend** Lülita sisse turvaline.

   > [!NOTE]
   > Microsoft tellib usaldusväärsete saatjate muude tootjate allikad. Kui turvaline loend on lubatud, ei märgita neid usaldusväärseid saatjaid ekslikult rämpspostiks. Soovitame selle suvandi valida, kuna see vähendab teile saadetud valepositiivsete (rämpspostiks liigitatud heade meilisõnumite) arvu.

Lisateavet leiate teemast Ühenduse [filtreerimise konfigureerimine.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy)
