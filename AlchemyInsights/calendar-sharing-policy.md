---
title: 618 kalendri ühiskasutuse poliitika
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/26/2020
ms.locfileid: "44372995"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Poliitika tõrge kalendri ühiskasutusse andmine

1. Tehke vastavalt oma olukorrale ühte järgmistest.
    - Kaugtöölaua PowerShelli abil ühendust Exchange Online ' i. Lisateabe saamiseks vaadake [ühendamine Exchange Online ' i kaugtöölaua PowerShelli abil](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Avage asutusesisese serveri Exchange Management shelli.
2. Määratlege ühiskasutuse poliitika, mis on määratud kasutajale. Selleks käivitage järgmine käsk ja Märkus tagastatud poliitika:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Värskendage kasutaja ühiskasutuse poliitika. Selleks tehke järgmist.
    - Avage Exchange ' i halduskeskus.
    - Klõpsake **organisatsioonija**seejärel topeltklõpsake poliitika, mis on määratud kasutaja **eraldi ühiskasutus**. See on poliitika, mis tagastati juhises 2.
    - Valige lehel ühiskasutuse reegel kalendri ühiskasutuse tase, mida soovite lubada jaotises **Määrake, millist teavet soovite jagada**; Klikkige nupul **Salvesta**.

Lisateabe saamiseks vaadake: ["poliitika ei luba anda õigusi sel tasemel ühe või mitme adressaadi (te)" tõrge, kui kasutaja proovib jagada kalendrit](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
