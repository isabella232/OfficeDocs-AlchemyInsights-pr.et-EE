---
title: Microsoft 365 rühma e-posti aadressi muutmine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/27/2020
ms.locfileid: "44282710"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a>Microsoft 365 rühma e-posti aadressi muutmine

Saate muuta Microsoft 365 rühma e-posti aadress admin Center abil. Valige lihtsalt rühm ja valige @edit e-posti aadress.

Võite kasutada ka EXO PowerShelli käsu abil saate muuta Microsoft 365 rühma esmane SMTP-aadress:

Komplekt-UnifiedGroup <Group Name> -PrimarySMTPAddress<new SMTP Address>

Näide:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
