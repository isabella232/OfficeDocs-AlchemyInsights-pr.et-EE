---
title: 'RBAC rollid '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583550"
---
# <a name="rbac-rules"></a>RBAC reeglid

Kui teil on õigus viga, tehke järgmist. 

- **Kliendil, kellel on objekti ID, ei ole lubatud ulatuses toiminguid teha (kood: AuthorizationFailed)**: kui proovite luua ressurssi, siis kontrollige, kas olete praegu sisse logitud kasutajaga, kellele on määratud roll, millel on valitud ulatuses ressursile kirjutamise õigus. Kui soovite näiteks hallata virtuaalseid masinaid ressursirühma, peaks teil olema ressursi rühmas (või vanemas ulatuses) [virtuaalarvuti kaastööline](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) roll. Iga sisseehitatud rolli kasutusõiguste loendi leiate teemast [Azure ' i ressursside sisseehitatud rollid](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- **Teil pole tugiteenuste taotluse loomise õigust**: kui proovite luua või värskendada tugiteenuse piletit, siis kontrollige, kas olete praegu sisse logitud kasutajaga, kellele on määratud Microsoft. support/supportTickets/Write õigus (nt [tugiteenuste taotluse kaastööd](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)).
- Rolli **ei saa enam määrata (kood: RoleAssignmentLimitExceeded)**: kui proovite rolli määrata, püüdke vähendada rollimäärangu arvu, määrates selle asemel rollid rühmadesse. Azure toetab kuni **2000** rolli määramist tellimuse kohta.

Azure ' i RBAC rollide kohta leiate lisateavet teemast [Azure ' i RBAC rollid](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
