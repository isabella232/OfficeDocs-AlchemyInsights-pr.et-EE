---
title: Kasutajate poliitikate/postkasti sätete parandamine
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
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746732"
---
# <a name="fix-user-policymailbox-settings"></a>Kasutajate poliitikate/postkasti sätete parandamine

Postkasti rämpsmeili sätted mõjutasid seda sõnumit. Sätete läbivaatamiseks tehke järgmist.

1. Käivitage Exchange Management shell. Lisateavet leiate teemast [Exchange ' i halduse kesta avamine](https://go.microsoft.com/fwlink/?linkid=2101432).
2. Käivitage see käsk (kasutaja meiliaadressi kasutamine):  **Get-mailboxjunkmailconfiguration-Identity "User@domain.com"**
3. Kontrollige, kas saatja meiliaadress on osa **TrustedSendersAndDomains** või **BlockedSendersAndDomains**. Kui meiliaadress on ühes loenditest, peate selle võib-olla eemaldama. Lisateavet leiate teemast [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
