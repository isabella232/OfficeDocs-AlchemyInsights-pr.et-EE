---
title: Tuvastada postkasti auditilogide väline e-posti saatmise
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7defd0902e8c8bebae9c7bfee72c3199cbc1909f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539097"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Tuvastada välise Meili edasisaatmine on konfigureeritud postkastide

Kui Office 365 kasutajale konfigureerib väliste meilide edasisaatmise funktsiooni postkast, auditeerib tegevuse osana cmdleti **Set-Mailbox** . Kuvatakse tegevuse turvalisuse & vastavuse Center auditi logifaili otsingu abil.

1. Logige sisse [Office 365 & vastavuse Turvakeskus](https://protection.office.com/).

2. Mine **Otsi** > **auditi logifaili** otsingulehte.

3. Valige kuupäevavahemik väljadele **Alguskuupäev** ja **lõppkuupäev** . Te ei pea määrama kasutajanime. Veenduge **tegevuse** välja näidata **kõigi tegevuste tulemusi**.

4. Klõpsake nuppu **Otsi**.

Tulemites klõpsake **Filtri tulemused** ja tippige **Set-Mailbox** väljale tegevuse filter. Valige kirjega auditi tulemused. Hüpik **üksikasjad** klõpsake **Lisateabe saamiseks**. Sa pead vaatama iga auditikirje kindlaks, kas tegevus on seotud e-posti edastamise üksikasjad.

- **ObjectId väärtuse**: alias väärtuse muutmise postkasti.

- **Parameetrid**: _ForwardingSmtpAddress_ näitab target e-posti aadress.

- **Kasutajanimi**: kasutaja konfigureeritud Meili edasisaatmine **ObjectId väärtuse** väljal postkastis.

Lisateabe saamiseks vt [Determining kes seadistada e-posti edasisuunamise postkasti](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
