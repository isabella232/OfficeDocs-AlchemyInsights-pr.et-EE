---
title: Välise automaatse meilisõnumite edasisaatmise blokeerimine või blokeeringu keelamine
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
ms.openlocfilehash: 6c4ddd53ab794ffad3179dd86a8f81785567cfe34240dff2aa0a1df11094883d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57897464"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>Meilisõnumite igavese automaatse edasisaatmise blokeerimine või blokeeringu tühistamiseks

Konkreetse postkasti jaoks meilisõnumite edasisaatmise lubamiseks või keelamiseks lugege teemat [Meilisõnumite edasisaatmise konfigureerimine.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Administraatorid saavad ettevõtte välist edasisaatmist juhtida väljamineva [rämpsposti poliitikate abil.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) Väljamineva rämpsposti poliitikaid saate hallata Microsoft 365 Defender <https://security.microsoft.com/antispam> PowerShelli [cmdlet-käsu Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) abil või Exchange Online kaudu.

Kui kuvatakse järgmine tõrketeade: **"550 5.7.520 Access denied, Your organization not allow external forwarding" ("550 5.7.520 Access denied, Your organization not allow external forwarding" ("550 5.7.520 Access denied, Your organization not allow external forwarding" ("550 5.7.520 Access denied),** teie ettevõte ei luba välist edasisaatmist", veenduge, et poliitika oleks konfigureeritud lubama väliseid automaatse edasisaatmise sõnumeid.

**Märkus.** Soovitame vaikeväärtust **Automaatne** –  süsteem, mida juhitakse automaatse edasisaatmise reeglite sättele väljamineva rämpsposti vaikepoliitikas (automaatne väline edasisaatmine on blokeeritud; sisemine automaatne edasisuunamine töötab endiselt). Peaksite looma kohandatud väljamineva rämpsposti filtri poliitikad ja kasutama väärtust **Sees – edasisaatmine** on lubatud ainult kasutajatele, kes vajavad välist automaatset meilisõnumite edasisaatmist. Lisateavet leiate teemast Välise [meilisõnumite edasisaatmise konfigureerimine Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).
