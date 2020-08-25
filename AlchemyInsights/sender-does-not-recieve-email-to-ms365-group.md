---
title: Saatja ei saa Microsoft 365 rühmale saadetud meilisõnumeid
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/21/2020
ms.locfileid: "46871758"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Saatja ei saa Microsoft 365 rühmale saadetud meilisõnumeid

Vaikimisi ei saa meilisõnumi saatja Microsoft 365 rühma sisendkaustas sõnumi koopiat, isegi kui saatja on rühma liige.

Kasutage seda EKSO PowerShelli käsku, et lubada saatjal saada koopia igast meilisõnumist, mille nad saadavad Microsoft 365 rühmale.  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Kõigi postkastide korraga häälestamise lubamiseks tehke järgmist.

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Märkus** Selle seadistuse muudatuste jõustumine võtab aega kuni tund.