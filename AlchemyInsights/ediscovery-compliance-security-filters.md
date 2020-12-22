---
title: Sisu otsingu/ekspordi ajal tulemeid ei tagastata
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727219"
---
# <a name="no-results-returned-during-content-searchexport"></a>Sisu otsingu/ekspordi ajal tulemeid ei tagastata

Kui teil esineb järgmisi e-juurdluse stsenaariumeid, tehke järgmist.

- Sisu otsimine/eksportimine ei tagasta andmeid ega ootamatuid andmeid
- e-juurdluse otsing või eksport nurjub

See võib olla tingitud teatud nõuetele vastavuse turbe filtritest, mis olid häälestatud teatud administraatori poolt ja mida pole kõigile administraatoritele edastatud.

Selle probleemi lahendamiseks kontrollige, kas on olemas nõuetele vastavuse turbe filtrid, mis võivad põhjustada järgmisi probleeme.

1. Ühenduse loomine turbe ja ühilduvuse keskusega PowerShell
2. Käivitage järgmine Commandlets.

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Lisateavet ühilduvuse turbe filtrite kohta leiate teemast [sisu otsimise õiguse filtreerimine](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
