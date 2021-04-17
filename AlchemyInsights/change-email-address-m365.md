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
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819076"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Microsoft 365 rühma või Microsoft Teamsi meiliaadressi muutmine

Microsoft 365 rühma või Microsoft Teamsi meiliaadressi muutmiseks saate kasutada [Microsoft 365 halduskeskust](https://admin.microsoft.com/). Selleks valige rühm ja seejärel @redigeeri meiliaadressi.

Microsoft 365 rühma või Teamsi peamise SMTP-aadressi muutmiseks saate kasutada ka järgmist EXO PowerShelli käsku:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Näide:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
