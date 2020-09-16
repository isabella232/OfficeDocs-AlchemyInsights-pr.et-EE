---
title: 2491 teatise meilisõnumid Phish, mis on tarnitud rentniku või kasutaja alistamise poliitika tõttu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728607"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Meilisõnumite teavitamine rentniku või kasutaja alistamise tõttu antud Phish

Vaike-teatise poliitika, mille nimi on "rentniku või kasutaja alistamise tõttu", on välja antud rentnikele, kellel on Office 365 ATP P1 ja P2 litsentsid. Kui saite teatise, saate uurida järgmisi juhiseid.

1. Klõpsake hoiatusteate nuppu **Kuva teatis** , et minna turbe & vastavuskontrolli lehe lehele **teatised** .

2. Valige teatis, et näha **sõnumite loendit** ja **vaadata sõnumeid Exploreris**. Mõlemad suvandid viivad teid sõnumi üksikasjade juurde, mis sisaldab sõnumi ID-dokumenti. Pange tähele, et ohu Exploreri link filtreerib automaatselt teatiste kriteeriumidele vastavaid sõnumeid. Võimalik, et peate täpsustama ohu Exploreris kuupäeva filtrit.

Andmepüügifilter edastati käsitsi konfigureeritud alistamise tõttu.

- Kasutaja määratud lubatud saatja või Domeen.

- Lubatud saatja või domeen, mille administraator on rämpsposti poliitikas määranud.

- Lubatud IP-aadress seoses filtri poliitikaga.

- Meilivoo reegel (tuntud ka kui transpordi reegel), mis on konfigureeritud sõnumite lubamiseks.

Kui arvate, et sõnum oli valesti märgitud kui Phish, kasutage meilisõnumite saatmiseks Microsoftile sõnumite saatmiseks Outlooki [aruannete lisandmoodulit](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) .
