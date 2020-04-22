---
title: 2491 hoiatus e-kirju "Phish tarnitud tõttu rentniku või kasutaja alistamine" poliitika
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758905"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Teavita e-kirju "Phish tarnitud tõttu rentniku või kasutaja alistamine" poliitika

Vaikimisi Alert poliitika nimega "Phish tarnitud tõttu rentniku või kasutaja alistamine" on välja antud rentnike Office 365 ATP P1 ja P2 litsentsid. Kui saite selle hoiatuse, on siin juhised uurimiseks.

1. Hoiatusteate, klõpsake nuppu **Kuva hoiatus** , et minna **hoiatuste** lehele Security & vastavuse keskus.

2. Valige teatis, et näha sõnumite **loendit** või **vaadata sõnumeid Exploreris**. Mõlemad suvandid viib teid sõnumi üksikasjadega, mis sisaldab sõnumi ID-ga. Pange tähele, et Ohuuurija link filtreerita automaatselt hoiatuskriteeriumidele vastavaid sõnumeid. Võimalik, et peate kohandama kuupäeva filtrit Threat Explorer.

Andmepüügiteade toimetati käsitsi konfigureeritud alistamise tõttu:

- Kasutaja määratud lubatud saatja või Domeen.

- Lubatud saatja või domeeni määratud administraatori Rämpspostivastane poliitika.

- Ühenduse filtripoliitika lubatud IP-aadress.

- Meilivoo reegel (tuntud ka kui transpordireegel), mis on konfigureeritud sõnumite lubamiseks.

Kui arvate, et sõnum oli valesti märgistatud Fish, kasutage Outlooki [aruande sõnumi lisandmoodul](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) edastada sõnumi näidised Microsoftile.
