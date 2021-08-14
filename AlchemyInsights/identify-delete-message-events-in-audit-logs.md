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
ms.openlocfilehash: f68b623abd0efa990df71e5bf1ea1c9e7367ed691b1752f68c971e973922a63d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57868414"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Kustutatud meilisõnumite logide auditeerimine

Alates jaanuarist 2019 lülitab Microsoft postkasti auditilogi vaikimisi sisse. Muul juhul peate konkreetse kasutaja kustutamissündmuste läbivaatamiseks käsitsi lubama auditeerimise kustutustoimingud. Kui postkasti auditilogi on teie asutuse või konkreetse kasutaja jaoks juba lubatud, järgige alltoodud juhiseid.

1. Logige sisse [Microsoft 365 vastavuskeskusesse](https://protection.office.com/)

2. Klõpsake **nuppu Otsing ja uurimine** ning valige **Auditilogi otsing.**

3. Valige väljadel Alguskuupäev **ja Lõppkuupäev** **kuupäevavahemik.** Määrake kasutaja kasutajanimi, keda soovite uurida (kasutaja, kes üksused kustutas). Valige väljal **Tegevused** kustutatud sõnumid **kaustast Kustutatud üksused ja** **Teisaldatud sõnumid kausta Kustutatud üksused.**

4. Klõpsake **nuppu Otsi**.

Valige tulemitest auditikirje. Klõpsake üksikasjade hüpiku jaotises nuppu **Lisateave.** Lisateavet kustutatud üksuse kohta (nt teemarida ja üksuse asukoht kustutamisel) kuvatakse väljal **AffectedItems.** Atribuut **ClientInfoString (ClientInfoString)** kuvatakse juhul, kui Outlook, Outlooki veebirakendus (varem tuntud kui Outlook Web App) või mis tahes muu seadmes.

Lisateavet leiate teemast [Postkasti jaoks meilisõnumite edasisaatmise häälestaja määratlemine.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)

**Märkus.** Auditilogi funktsiooni abil ei saa kustutatud üksusi tuua. Kustutatud sõnumite toomiseks Outlooki veebirakendus lugege [teemat Kustutatud üksuste taastamine Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
