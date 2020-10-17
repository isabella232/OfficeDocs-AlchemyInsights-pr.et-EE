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
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478313"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Meilisõnumite edasisaatmise blokeerimine või blokeeringu tühistamine

Mõne kindla postkasti meilisõnumite edasisaatmise lubamiseks või keelamiseks vaadake teemat [meilisõnumite edasisaatmise konfigureerimine](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Rentniku tasandil kontrollitakse välise edasisaatmise kontrolli väljamineva rämpsposti poliitika abil. Väljamineva rämpsmeili filtri poliitika saate vaadata turbe-ja vastavuskontrolli keskusest või [kasutada](https://protection.office.com/antispam) [käsku Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).

Kui kuvatakse järgmine tõrketeade: **"550 5.7.520 juurdepääs on keelatud, siis teie ettevõte ei luba välisedasisaatmist"**, veenduge, et poliitika oleks konfigureeritud välise automaatse edasisaatmise lubamiseks.

**Märkus:** Soovitatav on jätta väline Autoforward teie väljamineva rämpsmeili filtri poliitikas keelatud ja lubada seda ainult nende kasutajate jaoks, kes vajavad välisedasisaatmist, luues kohandatud poliitika nende kasutajate jaoks. Lisateavet leiate teemast [väliste meilisõnumite edasisaatmise konfigureerimine rakenduses Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).