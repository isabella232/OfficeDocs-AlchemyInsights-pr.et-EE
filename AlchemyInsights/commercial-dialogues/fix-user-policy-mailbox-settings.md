---
title: Kasutajapoliitika/postkasti sätete parandus
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
ms.openlocfilehash: fecc52bea66e0aed709a8995d2509f4432c09482459aa575d29e4c7551375211
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034714"
---
# <a name="fix-user-policymailbox-settings"></a>Kasutajapoliitika/postkasti sätete parandus

Seda sõnumit mõjutasid postkasti rämpspostisätted. Sätete läbivaatamiseks tehke järgmist.

1. Käivitage Exchange Management Shell. Lisateavet leiate teemast [Halduskesta Exchange avamine.](https://go.microsoft.com/fwlink/?linkid=2101432)
2. Käivitage see käsk (kasutades kasutaja meiliaadressi):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Kontrollige, kas saatja meiliaadress on **osa TrustedSendersAndDomainsist** või **BlockedSendersAndDomainsist.** Kui meiliaadress on ühes loendis, peate selle võib-olla eemaldama. Lisateavet leiate teemast [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
