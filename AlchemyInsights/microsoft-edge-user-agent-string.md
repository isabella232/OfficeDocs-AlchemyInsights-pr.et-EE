---
title: Microsoft Edge string (töölaud)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003862"
- "6914"
ms.openlocfilehash: 9311f17298fff3fee3282fe05bd1ddcd02780a80097e86b29d56ffd575a9a571
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975997"
---
# <a name="microsoft-edge-user-agent-string-desktop"></a>Microsoft Edge string (töölaud)

Kasutajaagendi (UA) stringe saab kasutada teatud opsüsteemis kasutatava konkreetse brauseri versiooni tuvastamiseks. Nagu teised brauserid, Microsoft Edge see teave http-päisesse "User-Agent" alati, kui ta saidilt taotluse esitab. Brauseri versiooniteabele pääseb juurde ka JavaScripti kaudu, küsides teksti "navigator.userAgent" väärtust.

Soovitame veebiarendajatel võimaluse korral kasutada funktsioonituvastust, et parandada koodi säilivust, vähendada koodi tundlikkust ja välistada koodikatkestuse oht edaspidiste UA stringivärskenduste korral.

Lisateavet leiate teemast [Microsoft Edge User Agent String (Desktop).](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string)