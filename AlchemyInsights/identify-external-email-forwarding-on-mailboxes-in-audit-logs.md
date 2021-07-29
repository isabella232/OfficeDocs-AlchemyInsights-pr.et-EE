---
title: Väliste meilisõnumite edasisaatmise tuvastamine auditilogides postkastides
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: b7146b2b09b6ac1e33b192dcbcbfb72ea2593313
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630245"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Väliste meilisõnumite edasisaatmise konfigureerimise tuvastamine postkastides

Kui Microsoft 365 konfigureerib postkastis välise meilisõnumite edasisaatmise, auditeeritakse tegevust **cmdlet-käsu Set-Mailbox osana.** Tegevusi saate vaadata auditilogi otsingu abil turbe- & vastavuskeskuses.

1. Logige sisse [Microsoft 365 vastavuskeskusesse.](https://protection.office.com/)

2. Avage leht **Otsi**  >  **auditilogi otsingut.**

3. Valige väljadel Alguskuupäev **ja Lõppkuupäev** **kuupäevavahemik.** Kasutajanime pole vaja määrata. Veenduge, **et välja** Tegevused väärtuseks oleks seatud Kõigi tegevuste **tulemite näitamine.**

4. Klõpsake **nuppu Otsi**.

Klõpsake tulemite väljal **Filtreeri tulemeid** ja tippige **väljale Tegevuse** filter käsk Sea postkast. Valige tulemitest auditikirje. Klõpsake **hüpiktekstis** Üksikasjad **nuppu Lisateave.** Selleks et teha kindlaks, kas tegevus on seotud meilisõnumite edasisaatmisega, peate vaatama iga auditikirje üksikasju.

- **ObjectId**: muudetud postkasti pseudonüüm.

- **Parameetrid:** _ForwardingSmtpAddress tähistab_ sihtmeiliaadressi.

- **UserId**: Kasutaja, kes konfigureeris meilisõnumite edasisaatmise väljal **ObjectId olevas postkastis.**

Lisateavet leiate teemast [Postkasti jaoks meilisõnumite edasisaatmise häälestaja määratlemine.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
