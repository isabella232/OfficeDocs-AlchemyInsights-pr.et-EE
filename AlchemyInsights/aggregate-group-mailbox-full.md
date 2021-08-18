---
title: AggregateGroupMailboxi täielik NDR,mis on vastu võetud Microsoft 365 rühmale saadetud meilisõnumite jaoks
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: ace8e256e3771f82512abcb9e20b832381eedf80
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315906"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailboxi täielik NDR,mis on vastu võetud Microsoft 365 rühmale saadetud meilisõnumite jaoks

Kasutage järgmist EXO Shelli käsku, et luua Exchange transpordireegel rühma koondpostkasti saadetud meilisõnumite vaikseks kukumiseks.

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

**Märkus.** Asendage **smtp-aadress jaotises -SentTo** oma rentniku koondrühma postkasti SMTP-aadressiga. Rühma koondpostkasti SMTP-aadressi saate kätte saadud NDR-i kaudu.



