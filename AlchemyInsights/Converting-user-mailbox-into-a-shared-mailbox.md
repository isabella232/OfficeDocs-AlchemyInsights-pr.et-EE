---
title: Kasutaja postkasti ümberarvestamisel ühiskasutuses postkasti?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496395"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a>Muuta kasutaja postkasti ühiskasutuses postkasti

Te saate teisendada ainult kasutaja postkasti ühiskasutuses postkasti kui kasutaja on Exchange litsents. Pärast teisendamist postkasti, ta jätkab näidata aktiivselt sest detsembri ühiskasutuses olevad postkastid. Siiski ümber postkasti ka kuvatakse loendis ühiskasutuses postkasti. 
  
Kui proovite muuta postkasti Exchange konsoolis ja teisendus nurjub, tühjendage brauseri vahemälu ja küpsised ja proovige uuesti. Kui see ikka ei tööta, proovige konverteeriva postkasti Exchange Management shelli poolt järgmise käsu:
  
```
Set-Mailbox -Type Shared
```

Postkasti konverteerimise Lisateave on esitatud [muuta kasutaja postkasti ühiskasutuses postkasti](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).
  
