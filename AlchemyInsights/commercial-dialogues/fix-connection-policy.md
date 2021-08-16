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
ms.openlocfilehash: 7eae77358b0305582f53c411a092e3d2f1dbe17fd58ceac1ac00d5c07b3dd202
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988087"
---
# <a name="fix-connection-policy"></a>Ühenduspoliitika parandus

Meilisõnum oli märgitud turvaliseks ja toimetati kasutaja sisendkausta, kuna saatva IP-aadressi märkimine ühendusefiltri poliitikas on turvaline. Poliitika läbivaatamiseks tehke järgmist.

1. Avage [Office 365 turbe- & ja](https://go.microsoft.com/fwlink/p/?linkid=2077143)seejärel valige Ohuhalduspoliitika   >    >  [rämpspostitõrje.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Valige **vahekaardil Kohandatud** ühendusefiltri poliitika **ja** seejärel valige **Redigeeri poliitikat**.
3. Vaadake **üle loend IP Allow (IP-luba).** Vaadake, **seif loend** on lubatud.

    > [!NOTE]
    > Microsoft tellib usaldusväärsete saatjate muude tootjate allikad. Kui **seif lubatud,** ei märgita neid usaldusväärseid saatjaid ekslikult rämpspostiks. Soovitame selle suvandi valida, kuna see vähendab teile saadetud valepositiivsete (rämpspostiks liigitatud heade meilisõnumite) arvu.
