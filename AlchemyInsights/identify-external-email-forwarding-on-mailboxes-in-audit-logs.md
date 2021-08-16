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
ms.openlocfilehash: 1e80917a323128ba23175651cdf4d892d7815a89c1223b654812c1b456c787da
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028730"
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
