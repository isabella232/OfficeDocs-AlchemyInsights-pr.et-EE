---
title: Omanik ei saa Outlooki abil alamkausta luua
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836131"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Omanik ei saa Outlooki abil alamkausta luua

**Avaliku kausta omanikel on käimas probleem alamkaustade loomisega Outlooki abil. Probleem lahendatakse peagi.**

Samal ajal kasutage ühte järgmistest lahendustest.

1. Outlook for MAC-i abil alamkausta loomine, kuna probleem mõjutab ainult Outlooki töölauaaknaid (kõiki versioone)
2. Kas administraator loob alamkausta EXO Shelli või EAC abil
3. Muutke kasutaja defaultPublicFolderMailbox/EffectivePublicFolderMailboxiks muuks postkastiks kui kausta sisupostkast, mis põhjustab probleemi  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Oodake tund, taaskäivitage Outlooki klientrakendus