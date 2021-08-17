---
title: 726 Meilisõnumite edasisaatmise blokeerimine
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
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059628"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Meilisõnumite edasisaatmise blokeerimine või blokeeringu tühistamiseks

Konkreetse postkasti jaoks meilisõnumite edasisaatmise lubamiseks või keelamiseks lugege teemat [Meilisõnumite edasisaatmise konfigureerimine.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Rentnikutasemel toimub välise edasisaatmise juhtimine väljamineva rämpsposti poliitika abil. Väljamineva rämpsposti filtri poliitikat saate vaadata turbe- [](https://protection.office.com/antispam) ja vastavuskeskuse kaudu siin või käsu [Get-HostedOutboundSpamFilterPolicy abil.](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)

Kui teile kuvatakse järgmine tõrketeade: **"550 5.7.520 Access denied, Your organization not allow external forwarding" ("550 5.7.520 Access denied, Your organization not allow external forwarding" ("550 5.7.520 Access denied,** Teie ettevõte ei luba välist edasisaatmist"), veenduge, et poliitika oleks konfigureeritud lubama välist automaatset edasisaatmist.

**Märkus.** Soovitatav on hoida väline automaatesitus teie väljamineva rämpsposti vaikefiltri poliitikas keelatud ja lubada see ainult kasutajatele, kes vajavad välist edasisaatmist, luues nende kasutajate jaoks kohandatud poliitika. Lisateavet leiate artiklist [Välise meilisõnumite edasisaatmise konfigureerimine Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)