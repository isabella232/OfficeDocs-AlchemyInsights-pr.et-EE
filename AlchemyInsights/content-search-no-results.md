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
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057998"
---
# <a name="no-results-from-content-searchexports"></a>Sisuotsingu/-ekspordi tulemid puuduvad

Sisuotsingu/ekspordiga seotud probleemid, mis ei tagasta andmeid, võivad olla tingitud teatud nõuetele vastavuse turbefiltrist, mille häälestas konkreetne administraator ja mis ei edastanud seda kõigile administraatoritele.

Probleemi lahendamiseks kontrollige, kas nõuetele vastavuse turbefiltrid võivad põhjustada seda.
1. Ühendus ja vastavuskeskuse PowerShelli kasutamine
2. Käivitage järgmised käsud.
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org