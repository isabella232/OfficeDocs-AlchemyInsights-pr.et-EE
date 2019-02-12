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
ms.openlocfilehash: 4da54121763fd33aa111f3bb3c26963cd271dc51
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906728"
---
Te saate teisendada ainult kasutaja postkasti ühiskasutuses postkasti kui kasutaja on Exchange litsents. Pärast teisendamist postkasti, ta jätkab näidata aktiivselt sest detsembri ühiskasutuses olevad postkastid. Siiski ümber postkasti ka kuvatakse loendis ühiskasutuses postkasti. 
  
Kui proovite muuta postkasti Exchange konsoolis ja teisendus nurjub, tühjendage brauseri vahemälu ja küpsised ja proovige uuesti. Kui see ikka ei tööta, proovige konverteeriva postkasti Exchange Management shelli poolt järgmise käsu:
  
```
Set-Mailbox -Type Shared
```

Postkasti konverteerimise Lisateave on esitatud [muuta kasutaja postkasti ühiskasutuses postkasti](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).
  
