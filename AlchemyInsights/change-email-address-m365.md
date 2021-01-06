---
title: Microsoft 365 rühma või Microsoft Teamsi meiliaadressi muutmine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756553"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Microsoft 365 rühma või Microsoft Teamsi meiliaadressi muutmine

Microsoft 365 rühma või Microsoft Teamsi meiliaadressi muutmiseks saate kasutada [Microsoft 365 halduskeskust](https://admin.microsoft.com/). Selleks valige rühm ja seejärel @redigeeri meiliaadressi.

Microsoft 365 rühma või Teamsi peamise SMTP-aadressi muutmiseks saate kasutada ka järgmist EXO PowerShelli käsku:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Näide:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
