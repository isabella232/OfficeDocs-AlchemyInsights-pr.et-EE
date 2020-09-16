---
title: Omanik ei saa Outlooki kaudu alamkausta luua
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665714"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Omanik ei saa Outlooki kaudu alamkausta luua

**On käimas probleem avalike kaustade omanikega, mis loovad Outlooki abil alamkaustad. Probleem lahendatakse varsti.**

Vahepeal kasutage ühte järgmistest lahendustest.

1. Rakenduse Outlook for MAC kasutamine alamkausta loomiseks kui probleem mõjutab ainult Outlooki töölaua Windowsi versiooni (kõik versioonid)
2. Administraator luua alamkaust, kasutades EKSO Shell või EAC
3. Kasutaja DefaultPublicFolderMailbox/EffectivePublicFolderMailbox muutmine teise postkasti, kui selle kausta sisu postkast on probleemi põhjustanud  
    - *Set-postkast user1 DefaultPublicFolderMailbox PubMBX3*
4. Oodake tund, taaskäivitage Outlooki klientrakendus