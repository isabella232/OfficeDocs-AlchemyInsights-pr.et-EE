---
title: Microsoft 365 rühma või Microsoft Teamsi meiliaadressi muutmine
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
ms.openlocfilehash: acb343553bfb7e100c03d0e7046ed5cbdd6b739b9a61e3faf17768bd8aadff34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995618"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Microsoft 365 rühma või Microsoft Teamsi meiliaadressi muutmine

Microsoft 365 rühma või Microsoft Teamsi meiliaadressi muutmiseks saate kasutada [Microsoft 365 halduskeskust](https://admin.microsoft.com/). Selleks valige rühm ja seejärel @redigeeri meiliaadressi.

Microsoft 365 rühma või Teamsi peamise SMTP-aadressi muutmiseks saate kasutada ka järgmist EXO PowerShelli käsku:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Näide:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
