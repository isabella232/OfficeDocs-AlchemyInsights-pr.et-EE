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
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819040"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Microsoft 365 rühma meiliaadressi muutmine

Microsoft 365 rühma meiliaadressi saate muuta halduskeskuse kaudu. Selleks valige rühm ja seejärel @redigeeri meiliaadressi.

Microsoft 365 rühma peamise SMTP-aadressi muutmiseks saate kasutada ka järgmist EXO PowerShelli käsku:

Set-UnifiedGroupi <Group Name> -PrimarySmtpAddress <new SMTP Address>

Näide:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
