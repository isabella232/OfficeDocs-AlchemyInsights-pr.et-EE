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
ms.openlocfilehash: aa0ff925ae891d28e31394ec66eb17c2d9710008
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429479"
---
# <a name="turn-on-mailbox-auditing"></a>Postkasti auditeerimise sisselülitamine

Kui soovite postkasti auditeerimise lülitada ühe kasutaja või kogu asutuse jaoks, käivitage Remote PowerShelli kaudu järgmised cmdlet-käsud.

- **Üks kasutaja**: Set-Mailbox-identiteet "Jane Dow"-AuditEnabled $True
- **Ettevõte**: Get-Mailbox-ResultSize Unlimited-filter {RecipientTypeDetails-EQ "UserMailbox"} | Set-Mailbox-AuditEnabled $true

Lisateavet leiate teemast [postkasti auditeerimise haldamine](https://go.microsoft.com/fwlink/?linkid=2103668).