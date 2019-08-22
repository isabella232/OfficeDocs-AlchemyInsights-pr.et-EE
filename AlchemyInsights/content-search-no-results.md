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
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516775"
---
# <a name="no-results-from-content-searchexports"></a>Tulemeid: sisu otsing/eksport

Küsimused koos sisu otsing/eksport ei tule mingeid andmeid võib olla tingitud teatud konkreetsete Admin ja ei suhtle kõigile administraatoritel setup vastavuse turvalisusefiltrit.

Probleemi lahendamiseks kontrollige, kas täitmise turvalisuse filtreid, mis võivad põhjustada see:
1. Turvalisus ja vastavus Center PowerShelli ühendamine
2. Käivitage järgmine cmdlet-käsud:
<br>$org = "teiedomeen.com"
<br>Get-ComplianceSecurityFilter-organisatsiooni $org