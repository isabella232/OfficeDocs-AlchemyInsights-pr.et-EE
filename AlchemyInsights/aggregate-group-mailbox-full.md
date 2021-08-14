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
ms.openlocfilehash: 6655bbe9482400eeb3cfdf0b91bdc595e3d98fbff0f6d9244db8bb4dd958305e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951849"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailboxi täielik NDR,mis on vastu võetud Microsoft 365 rühmale saadetud meilisõnumite jaoks

Kasutage järgmist EXO Shelli käsku, et luua Exchange transpordireegel rühma koondpostkasti saadetud meilisõnumite vaikseks kukumiseks.

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> Asendage smtp-aadress jaotises **-SentTo** oma rentniku koondrühma postkasti SMTP-aadressiga. Rühma koondpostkasti SMTP-aadressi saate kätte saadud NDR-i kaudu.



