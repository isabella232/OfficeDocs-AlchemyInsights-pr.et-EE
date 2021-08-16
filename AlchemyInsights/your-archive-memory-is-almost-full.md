---
title: Arhiivipostkast on peaaegu täis
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046748"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Arhiivipostkast on peaaegu täis

Kui kasutaja saab hoiatuse; **Arhiivipostkast on peaaegu täis** või peate nende arhiivipostkasti mahtu suurendama. Siin on mõned näpunäited.

1. Kui kasutajale on määratud Exchange Online leping 1, **uuendage Exchange Online leping 2** litsentsile, et suurendada mahtu 50 GB-lt 100 GB-le.
1. Kui kasutajale on juba määratud üks järgmistest: **Exchange Online leping 2** või Exchange Online leping 1 koos Exchange Online'i arhiivimisteenus lisandmooduliga, kasutage automaatse arhiivimise lubamiseks järgmisi juhiseid.
 
    1. [Ühendus powershelli Exchange Online .](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)
    2. Käivitage kasutaja jaoks järgmine käsk:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Käivitage järgmine käsk, et kinnitada, et see on kasutaja jaoks lubatud.  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Lisateavet leiate teemast

- [Piiramatu arhiivimise lubamine – administraatori spikker – Microsoft 365 nõuetele | Microsoft Docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online piirangud – teenusekirjeldused | Microsoft Docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Üleminek muule äriplaanile | Microsoft Docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

