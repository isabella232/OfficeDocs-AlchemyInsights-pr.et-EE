---
title: Ühenduste poliitika parandamine
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746747"
---
# <a name="fix-connection-policy"></a>Ühenduste poliitika parandamine

Meilisõnum oli märgitud turvaliseks ja toimetatakse kasutaja sisendkausta, kuna saatmise IP-aadress oli märgitud turvaliseks filtri poliitikas. Poliitika läbivaatamiseks tehke järgmist.

1. Minge [Office 365 turbe & nõuetele vastavuse keskusse](https://go.microsoft.com/fwlink/p/?linkid=2077143)ja seejärel valige **ohustatud halduse**  >  **poliitika**  >  [anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Valige vahekaardil **kohandatud** **filtri poliitika** ja seejärel valige **Redigeeri poliitikat**.
3. Vaadake üle **IP-lubatute** loend. Vaadake, kas **turvaline loend** on lubatud.

    > [!NOTE]
    > Microsoft tellib usaldusväärsete saatjate kolmanda osapoole allikaid. Kui **turvaline loend** on lubatud, pole need usaldusväärsed saatjad ekslikult rämpspostina märgitud. Soovitan valida selle suvandi, sest see vähendab valede positiivsete (hea meili, mis on klassifitseeritud rämpspostiks) arvu.
