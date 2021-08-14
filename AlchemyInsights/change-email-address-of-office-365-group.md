---
title: Microsoft 365 rühma meiliaadressi muutmine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 6bd9301b983d09f6a0058fee17577b9fc695458ed205f96aacf79a87e4a91e34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930725"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Microsoft 365 rühma meiliaadressi muutmine

Microsoft 365 rühma meiliaadressi saate muuta halduskeskuse kaudu. Selleks valige rühm ja seejärel @redigeeri meiliaadressi.

Microsoft 365 rühma peamise SMTP-aadressi muutmiseks saate kasutada ka järgmist EXO PowerShelli käsku:

Set-UnifiedGroupi <Group Name> -PrimarySmtpAddress <new SMTP Address>

Näide:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
