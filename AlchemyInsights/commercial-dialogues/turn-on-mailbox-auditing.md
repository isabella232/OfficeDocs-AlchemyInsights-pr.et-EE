---
title: Postkasti auditeerimise sisselülitamine
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 797dd57aaa43e879c015a36c79c8c9fb13e04ae894b33b0f7c6d9694d1ae1960
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058034"
---
# <a name="turn-on-mailbox-auditing"></a>Postkasti auditeerimise sisselülitamine

Postkasti auditeerimise sisselülimiseks ühe kasutaja või kogu ettevõtte jaoks käivitage Remote PowerShelli kaudu järgmised cmdlet-käsud.

- **Üksikkasutaja**: Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true
- **Ettevõte:** Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true

Lisateavet leiate teemast [Postkasti auditeerimise haldamine.](https://go.microsoft.com/fwlink/?linkid=2103668)