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
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 518e4dd485ee7c54ce83e65794152e32f4c3a836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34751995"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Tuvastada välise Meili edasisaatmine on konfigureeritud postkastide

Kui kasutaja konfigureerib väliste meilide edasisaatmise funktsiooni postkast, auditeerib tegevuse osana cmdleti **Set-Mailbox** . Kuvatakse tegevuse turvalisuse & vastavuse Center auditi logifaili otsingu abil.

1. Logige sisse [Office 365 & vastavuse Turvakeskus](https://protection.office.com/)

2. Valige **Auditi logifaili Otsi**nuppu **Otsi ja uurimine** .

3. Valige kuupäevavahemik väljadele **Alguskuupäev** ja **lõppkuupäev** . Te ei pea määrama kasutajanime. Veenduge **tegevuse** välja näidata **kõigi tegevuste tulemusi**.

4. Klõpsake nuppu **Otsi**.

Tulemites klõpsake **Filtri tulemused** ja tippige **Set-Mailbox** väljale tegevuse filter. Valige kirjega auditi tulemused. Hüpik **üksikasjad** klõpsake **Lisateabe saamiseks**. Sa pead vaatama iga auditikirje kindlaks, kas tegevus on seotud e-posti edastamise üksikasjad.

- **ObjectId väärtuse**: alias väärtuse muutmise postkasti.

- **Parameetrid**: _ForwardingSmtpAddress_ näitab target e-posti aadress.

- **Kasutajanimi**: kasutaja konfigureeritud Meili edasisaatmine **ObjectId väärtuse** väljal postkastis.

Lisateabe saamiseks vt [Determining kes seadistada e-posti edasisuunamise postkasti](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
