---
title: Sisu otsing tulemeid
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680643"
---
# <a name="no-results-from-content-searchexports"></a>Sisu otsingu/ekspordi tulemeid ei kuvata

Sisu otsimisega/ekspordiga seotud probleemid võivad olla tingitud teatud nõuetele vastavuse turbe filtrist, mis on häälestatud teatud administraatori poolt ja mitte edastama seda kõigile administraatoritele.

Selle probleemi lahendamiseks kontrollige, kas selle põhjuseks võib olla mõni nõuetele vastav turvamise filtrid.
1. Ühenduse loomine turbe ja ühilduvuse keskusega PowerShell
2. Käivitage järgmine Commandlets.
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-organisatsioon $org