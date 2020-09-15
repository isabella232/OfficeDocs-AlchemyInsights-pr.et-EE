---
title: Tuvasta sõnumi sündmuste kustutamine auditi logides
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696509"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Kustutatud meilisõnumite auditi logid

Alates jaanuarist 2019 on Microsoft vaikimisi Postkasti auditilogi sisse lülitanud. Vastasel juhul peate kindla kasutaja jaoks sõnumite kustutamise üle vaatamiseks käsitsi lubama toimingute kustutamise. Kui postkasti auditi logimine on teie asutuse või konkreetse kasutaja jaoks juba lubatud, järgige alltoodud juhiseid.

1. Logige sisse [Microsoft 365 turbe & nõuetele vastavuse keskuses](https://protection.office.com/)

2. Klõpsake nuppu **Otsing ja juurdlus** ning valige **auditilogi otsing**.

3. Valige väljadel **Alguskuupäev** ja **lõppkuupäev** kuupäevavahemik. Määrake kasutaja kasutajanimi, mida soovite uurida (üksuste kustutanud kasutaja). Valige väljal **Tegevused** **kaust** kustutatud ja **teisaldatud sõnumid kausta Kustutatud üksused**.

4. Klõpsake nuppu **Otsi**.

Valige tulemites auditi kirje. Klõpsake hüpik üksikasjad nuppu **veel teavet**. Väljal **AffectedItems** kuvatakse Lisateave kustutatud üksuse kohta (nt üksuse teemarida ja üksuse asukoht, kui see kustutati). Atribuut **ClientInfoString** kuvatakse siis, kui kustutatud on Outlookis, Outlooki veebirakenduses (varem Outlook Web App) või mis tahes muus seadmes.

Lisateavet leiate teemast [postkasti jaoks meili edasisaatmise häälestamine](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Märkus**: kustutatud üksusi ei saa auditi Logi funktsiooni abil taastada. Outlooki veebirakenduses kustutatud sõnumite toomise kohta leiate teavet teemast [Kustutatud üksuste taastamine Outlook Web Appis](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
