---
title: Sisu otsida tulemeid
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800298"
---
# <a name="no-results-from-content-searchexports"></a>Tulemeid: sisu otsing/eksport

Küsimused koos sisu otsing/eksport ei tule mingeid andmeid võib olla tingitud teatud konkreetsete Admin ja ei suhtle kõigile administraatoritel setup vastavuse turvalisusefiltrit.

Probleemi lahendamiseks kontrollige, kas täitmise turvalisuse filtreid, mis võivad põhjustada see:
1. Turvalisus ja vastavus Center PowerShelli ühendamine
2. Käivitage järgmine cmdlet-käsud:
<br>$org = "teiedomeen.com"
<br>Get-ComplianceSecurityFilter-organisatsiooni $org