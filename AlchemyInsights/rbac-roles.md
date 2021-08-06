---
title: 'RBAC-rollid '
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
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923127"
---
# <a name="rbac-rules"></a>RBAC-reeglid

Kui kuvatakse õigusetõrge: 

- **Objekti ID-ga** klientrakendusel pole õigust teha toimingut ulatuse üle (kood: Autoriseerimine nurjus) : kui proovite luua ressurssi, kontrollige, kas olete praegu sisse logitud kasutajaga, kellele on määratud roll, kellel on valitud ulatuses ressursile kirjutamisõigus. Näiteks virtuaalarvutite haldamiseks ressursirühmas peaks teil [](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) olema ressursirühmas (või emaulatuses) virtuaalarvuti kaasautori roll. Iga valmisrolli õiguste loendi leiate teemast [Azure'i ressursside sisseehitatud rollid.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)
- **Teil pole** tugiteenusetaotluse loomise õigust. Kui proovite luua või värskendada tugiteenusepiletit, kontrollige, kas olete praegu sisse logitud kasutajaga, kellele on määratud Microsoft.Support/supportTickets/write õigus [(nt](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)tugiteenusetaotluse kaasautor).
- Rohkem rollimääranguid ei saa luua **(kood: RoleAssignmentLimitExceeded)**– kui proovite rolli määrata, proovige rolliülesannete arvu vähendada, määrates rollid rühmadele. Azure toetab kuni **2000** rollimäärangut tellimuse kohta.

Lisateavet Azure RBAC rollide kohta leiate teemast [Azure RBAC rollid.](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)
