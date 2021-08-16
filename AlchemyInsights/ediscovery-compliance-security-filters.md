---
title: Sisuotsingu/-ekspordi käigus ei tagastata tulemiid
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
ms.openlocfilehash: 5c04364f98dccbcad0f011df866f137d79c166ad3839b408d6be447d50a87ac3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101262"
---
# <a name="no-results-returned-during-content-searchexport"></a>Sisuotsingu/-ekspordi käigus ei tagastata tulemiid

Kui teil on probleeme järgmiste e-juurdluse stsenaariumidega:

- Sisuotsing/eksportimine ei tagasta andmeid ega ootamatuid andmeid
- e-juurdluse otsing või eksportimine nurjub

See võib olla tingitud teatud nõuetele vastavuse turbefiltritest, mille häälestas konkreetne administraator ja mida ei ole kõigile administraatoritele edastatud.

Probleemi lahendamiseks kontrollige, kas mõni nõuetele vastavuse turbefiltreid võib põhjustada järgmisi probleeme.

1. Ühendus ja vastavuskeskuse PowerShelli kasutamine
2. Käivitage järgmised käsud.

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Lisateavet nõuetele vastavuse turbefiltrite kohta leiate teemast [Sisuotsingu õiguste filtreerimine](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
