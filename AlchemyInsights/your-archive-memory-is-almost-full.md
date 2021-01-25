---
title: Teie arhiivi postkast on peaaegu täis
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
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974277"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Teie arhiivi postkast on peaaegu täis

Kui kasutaja saab hoiatuse; **Teie arhiivi postkast on peaaegu täis** või peate suurendama arhiivi postkasti mahtu, siin on mõned näpunäited.

1. Kui kasutajale on määratud Exchange Online ' i leping 1, üleminekuks **Exchange Online ' i** lepingule 2 litsentsi suurendamiseks 50 GB-st kuni 100GB.
1. Kui kasutaja on juba määratud ühte järgmistest: **Exchange Online ' i leping 2** või Exchange Online ' i leping 1 koos Exchange Online ' i arhiivimise lisandmooduliga, kasutage allolevaid juhiseid, et lubada automaatne laiendamine arhiivimine:.
 
    1. [Ühenduse loomine Exchange Online PowerShelliga](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Käivitage kasutaja jaoks järgmine unifiedgroup.  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Kasutajale lubatud kinnitamiseks käivitage järgmine unifiedgroup.  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Lisateavet leiate järgmistest teemadest.

- [ Luba piiramatu arhiveerimine – administraatori spikker – Microsoft 365 nõuetele vastavus | Microsoft docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online ' i limiidid – teenuste kirjeldused | Microsoft docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Üleminek mõnele muule äriplaanile | Microsoft docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

