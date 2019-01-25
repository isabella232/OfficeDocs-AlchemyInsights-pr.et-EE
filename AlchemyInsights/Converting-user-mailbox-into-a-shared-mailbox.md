---
title: Kasutaja postkasti ümberarvestamisel ühiskasutuses postkasti?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Priority
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 22ad1b3fb818b40bcd77974031735f931e986968
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29466260"
---
Te saate teisendada ainult kasutaja postkasti ühiskasutuses postkasti kui kasutaja on Exchange litsents. Pärast teisendamist postkasti, ta jätkab näidata aktiivselt sest detsembri ühiskasutuses olevad postkastid. Siiski ümber postkasti ka kuvatakse loendis ühiskasutuses postkasti. 
  
Kui proovite muuta postkasti Exchange konsoolis ja teisendus nurjub, tühjendage brauseri vahemälu ja küpsised ja proovige uuesti. Kui see ikka ei tööta, proovige konverteeriva postkasti Exchange Management shelli poolt järgmise käsu:
  
```
Set-Mailbox -Type Shared
```

Postkasti konverteerimise Lisateave on esitatud [muuta kasutaja postkasti ühiskasutuses postkasti](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).
  
