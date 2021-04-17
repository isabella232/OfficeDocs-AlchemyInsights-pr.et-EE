---
title: Sisuotsing tulemiteta
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816844"
---
# <a name="no-results-from-content-searchexports"></a>Sisuotsingu/-ekspordi tulemid puuduvad

Sisuotsingu/ekspordiga seotud probleemid, mis ei tagasta andmeid, võivad olla tingitud teatud nõuetele vastavuse turbefiltrist, mille häälestas konkreetne administraator ja mis ei edastanud seda kõigile administraatoritele.

Probleemi lahendamiseks kontrollige, kas nõuetele vastavuse turbefiltrid võivad põhjustada seda.
1. Ühenduse loomine turbe- ja vastavuskeskuse PowerShelliga
2. Käivitage järgmised käsud.
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org