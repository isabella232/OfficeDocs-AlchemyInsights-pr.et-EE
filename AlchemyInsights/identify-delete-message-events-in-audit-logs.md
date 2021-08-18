---
title: Auditilogides sõnumisündmuste kustutamise tuvastamine
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
ms.openlocfilehash: 7e13c9e5fbfa6ade065c2810150687085c1a9daae1a11c134688ec9a83ad37d9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54115644"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Kustutatud meilisõnumite logide auditeerimine

Alates jaanuarist 2019 lülitab Microsoft postkasti auditilogi vaikimisi sisse. Muul juhul peate konkreetse kasutaja kustutamissündmuste läbivaatamiseks käsitsi lubama auditeerimise kustutustoimingud. Kui postkasti auditilogi on teie asutuse või konkreetse kasutaja jaoks juba lubatud, järgige alltoodud juhiseid.

1. Logige sisse [Microsoft 365 vastavuskeskusesse](https://protection.office.com/)

2. Klõpsake **nuppu Otsing ja uurimine** ning valige **Auditilogi otsing.**

3. Valige väljadel Alguskuupäev **ja Lõppkuupäev** **kuupäevavahemik.** Määrake kasutaja kasutajanimi, keda soovite uurida (kasutaja, kes üksused kustutas). Valige väljal **Tegevused** kustutatud sõnumid **kaustast Kustutatud üksused ja** **Teisaldatud sõnumid kausta Kustutatud üksused.**

4. Klõpsake **nuppu Otsi**.

Valige tulemitest auditikirje. Klõpsake üksikasjade hüpiku jaotises nuppu **Lisateave.** Lisateavet kustutatud üksuse kohta (nt teemarida ja üksuse asukoht kustutamisel) kuvatakse väljal **AffectedItems.** Atribuut **ClientInfoString** kuvatakse, kui kustutamine toimus Outlook, Outlooki veebirakendus (varem Outlook Web App) või mis tahes muu seadmega.

Lisateavet leiate teemast [Postkasti jaoks meilisõnumite edasisaatmise häälestaja määratlemine.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)

**Märkus.** Auditilogi funktsiooni abil ei saa kustutatud üksusi tuua. Kustutatud sõnumite toomiseks Outlooki veebirakendus lugege [teemat Kustutatud üksuste taastamine Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
