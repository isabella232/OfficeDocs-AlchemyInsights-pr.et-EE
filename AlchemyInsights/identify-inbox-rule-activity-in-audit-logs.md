---
title: Sisendkausta reeglitegevuse tuvastamine auditilogides
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: e27c6433c65079af93f2a02a998b7179222336b0cae1149f4196f6fb6558ddac
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53976861"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Sisendkausta reeglitegevuse tuvastamine auditilogides

Sisendkausta reeglisündmuste (sisendkaustareeglite loomine, muutmine ja kustutamine) vaatamiseks saate Microsoft 365 turbekontrolli & auditilogi otsingut.

1. Logige sisse [Microsoft 365 vastavuskeskusesse.](https://protection.office.com/)

2. Avage leht **Otsi**  >  **auditilogi otsingut.**

3. Valige väljadel Alguskuupäev **ja Lõppkuupäev** **kuupäevavahemik.**

4. **Veenduge Exchange jaotises Postkastitegevused** on välja **Tegevused** väärtuseks seatud **New-InboxRule Create/modify/enable/disable inbox rule**.

5. Klõpsake **nuppu Otsi**.

Valige tulemitest auditikirje. Klõpsake üksikasjade hüpiku jaotises nuppu **Lisateave.** Teave sisendkausta reegli sätete kohta kuvatakse väljal **Parameetrid.**

Lisateavet leiate teemast Sisendkaustareegli [loomise kindlaksmääramine](/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
