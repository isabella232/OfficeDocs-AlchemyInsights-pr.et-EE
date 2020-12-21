---
title: Microsoft 365 rühmale saadetud meilisõnumite jaoks vastuvõetud AggregateGroupMailbox täielik NDR
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
ms.openlocfilehash: 9de09ab4cbd2f09648305b11da6273ed990907cf
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/18/2020
ms.locfileid: "49721821"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>Microsoft 365 rühmale saadetud meilisõnumite jaoks vastuvõetud AggregateGroupMailbox täielik NDR

Kasutage järgmisi EKSO Shell käsku Exchange ' i transpordi reegli loomiseks, et meilisõnumid saadetaks kokku rühma postkasti.

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> Asendage oma rentniku jaoks SMTP **-aadress SentTo SMTP-** aadressiga. Saate hankida kogu rühma postkasti SMTP-aadressi saadud NDR-ist.



