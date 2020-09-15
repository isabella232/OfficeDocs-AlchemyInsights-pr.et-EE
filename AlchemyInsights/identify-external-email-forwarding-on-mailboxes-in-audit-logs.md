---
title: Väliste meilisõnumite edasisaatmise tuvastamine auditi logide postkastides
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
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696293"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Tuvastamine, kui väline meilisõnumite edasisaatmine on konfigureeritud postkastides

Kui Microsoft 365 kasutaja konfigureerib välise meili edasisaatmise postkastis, auditeeritakse tegevust cmdlet **-käsu Set-Mailbox** osana. Auditilogi abil saate vaadata tegevust turbe & vastavuskontrolli keskuses.

1. Logige sisse [Microsoft 365 turbe & nõuetele vastavuse keskuses](https://protection.office.com/).

2. Avage leht **Otsingu**  >  **auditilogi otsing** .

3. Valige väljadel **Alguskuupäev** ja **lõppkuupäev** kuupäevavahemik. Te ei pea kasutajanime määrama. Veenduge, et väli **Tegevused** oleks seatud **kõigi tegevuste tulemite kuvamiseks**.

4. Klõpsake nuppu **Otsi**.

Klõpsake tulemites nuppu **Filtreeri tulemid** ja tippige väljale tegevuse filter **väärtus Set-postkast** . Valige tulemites auditi kirje. Klõpsake hüpik **üksikasjad** nuppu **veel teavet**. Peate iga auditi kirje üksikasju uurima, et teha kindlaks, kas tegevus on seotud meilisõnumite edasisaatmisega.

- **ObjectId**: muudetud postkasti pseudonüümi väärtus.

- **Parameetrid**: _ForwardingSmtpAddress_ tähistab TARGETi meiliaadressi.

- **Kasutajanimi**: kasutaja, kes konfigureeris meilisõnumite edasisaatmise väljal **ObjectId** postkastis.

Lisateavet leiate teemast [postkasti jaoks meili edasisaatmise häälestamine](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
