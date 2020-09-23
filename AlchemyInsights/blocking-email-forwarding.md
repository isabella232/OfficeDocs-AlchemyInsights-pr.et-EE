---
title: 726 meilisõnumite edasisaatmise blokeerimine
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219851"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Meilisõnumite edasisaatmise blokeerimine või blokeeringu tühistamine

Mõne kindla postkasti meilisõnumite edasisaatmise lubamiseks või keelamiseks vaadake teemat [meilisõnumite edasisaatmise konfigureerimine](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Rentniku tasandil kontrollitakse välise edasisaatmise kontrolli väljamineva rämpsposti poliitika abil. Kui see on välja lülitatud või automaatne, võib see blokeerida meilisõnumite edasisaatmise "550 5.7.520 juurdepääs keelatud, teie ettevõte ei luba välist edasisaatmist". Seejärel, kui edasisaatmine oli seatud blokeerima, on see viga, mida kasutajad näevad.

Kui edasisaatmine on blokeeritud, veenduge, et poliitika oleks konfigureeritud väliste Autoforward lubamiseks. Väljamineva rämpsmeili filtri poliitika saate kontrollida turbe-ja vastavuskontrolli keskusest või käivitades käsu Get-HostedOutboundSpamFilterPolicy | välgu nimi, AutoForwardingMode. Kui soovite häälestada Autoforward blokeerimist, siis ütleb sama käsk teile kohe poliitika oleku.

Märkus: soovitatav on jätta välist Autoforward teie väljamineva rämpsmeili filtri poliitikas keelatud ja lubada seda ainult nende kasutajate jaoks, kes vajavad välisedasisaatmist, luues kohandatud poliitika nende kasutajate jaoks. Lisateavet leiate teemast [väliste meilisõnumite edasisaatmise konfigureerimine rakenduses Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).