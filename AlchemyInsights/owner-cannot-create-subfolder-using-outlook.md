---
title: Omanik ei saa alamkausta luua Outlook
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
ms.openlocfilehash: 60190727e75c120ad3915da8b563b7f6b1a3238b46bb6e14cbf956365e1a84e0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54063120"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Omanik ei saa alamkausta luua Outlook

**Avalike kaustade omanikel on pidevalt probleem alamkaustade loomisega, kasutades Outlook. Probleem lahendatakse peagi.**

Samal ajal kasutage ühte järgmistest lahendustest.

1. Kasutage Outlook for MAC alamkausta loomiseks, kuna probleem mõjutab ainult Outlook (kõik versioonid)
2. Kas administraator loob alamkausta EXO Shelli või EAC abil
3. Muutke kasutaja defaultPublicFolderMailbox/EffectivePublicFolderMailboxiks muuks postkastiks kui kausta sisupostkast, mis põhjustab probleemi  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Oodake tund, taaskäivitage Outlooki klientrakendus