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
ms.openlocfilehash: 48634fad8f573e3a7c38cac299bb95ec90814f5c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331155"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Väliste meilisõnumite edasisaatmise konfigureerimise tuvastamine postkastides

Kui Microsoft 365 konfigureerib postkastis välise meilisõnumite edasisaatmise, auditeeritakse tegevust **cmdlet-käsu Set-Mailbox osana.** Tegevus on näha auditilogi otsingu abil. Selleks tehke järgmist.

1. Tehke ühte järgmistest toimingutest.
   - Avage Microsoft 365 vastavuskeskus lahenduste audit <https://compliance.microsoft.com>  \> . Või otse lehele Auditeeri **minemiseks** kasutage funktsiooni <https://compliance.microsoft.com/auditlogsearch> .
   - Avage Microsoft 365 Defender portaalis <https://security.microsoft.com> **Audit**. Või otse lehele Auditeeri **minemiseks** kasutage funktsiooni <https://sip.security.microsoft.com/auditlogsearch> .

2. Kontrollige **lehel** Audit, kas vahekaart **Otsing** on valitud, ja seejärel konfigureerige järgmised sätted.
   - Valige väljadele Algus ja Lõpp **kuupäeva-/kellaajavahemik.** 
   - Veenduge, **et väli Tegevused** **sisaldaks kõigi tegevuste tulemite kuvamist.**

3. Kui olete lõpetanud, klõpsake nuppu **Otsi**. Tegevused kuvatakse uuel lehel **Auditiotsing.**

4. Klõpsake tulemite väljal **Filtreeri tulemeid** ja tippige **väljale Tegevuse** filter käsk Sea postkast.

5. Valige tulemitest auditikirje. Klõpsake **hüpiktekstis** Üksikasjad **nuppu Lisateave.** Selleks et teha kindlaks, kas tegevus on seotud meilisõnumite edasisaatmisega, peate vaatama iga auditikirje üksikasju.

   - **ObjectId**: muudetud postkasti pseudonüüm.
   - **Parameetrid:** _ForwardingSmtpAddress tähistab_ sihtmeiliaadressi.
   - **UserId**: Kasutaja, kes konfigureeris meilisõnumite edasisaatmise väljal **ObjectId olevas postkastis.**

Lisateavet leiate teemast [Postkasti jaoks meilisõnumite edasisaatmise häälestaja määratlemine.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
