---
title: Omanik ei saa outlooki abil alamkausta luua
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/12/2020
ms.locfileid: "44748905"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Omanik ei saa outlooki abil alamkausta luua

**Käimas on probleem ühiskaustade omanike loomine alamkaustad Outlooki abil. Küsimus lahendatakse varsti.**

Vahepeal kasutage ühte järgmistest lahendused:

1. Kasutage Outlooki mac-i alamkausta loomiseks, kuna probleem mõjutab ainult Outlooki töölauaakende jaoks (kõik versioonid)
2. Kas admin luua alamkausta kasutades EXO Shell või EAC
3. Muutke DefaultPublicFolderMailbox/EffectivePublicFolderMailbox kasutaja muu postkasti kui sisu postkasti probleemi põhjustava kausta  
    - *Set-postkasti kasutaja1 DefaultPublicFolderMailbox PubMBX3*
4. Oodake tund, taaskäivitage Outlooki klient