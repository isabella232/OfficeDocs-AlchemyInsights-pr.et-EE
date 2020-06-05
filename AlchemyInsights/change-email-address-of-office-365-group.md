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
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580653"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Microsoft 365 rühma e-posti aadressi muutmine

Saate muuta Microsoft 365 rühma e-posti aadress admin Center abil. Valige lihtsalt rühm ja valige @edit e-posti aadress.

Võite kasutada ka EXO PowerShelli käsu abil saate muuta Microsoft 365 rühma esmane SMTP-aadress:

Komplekt-UnifiedGroup <Group Name> -PrimarySMTPAddress<new SMTP Address>

Näide:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
