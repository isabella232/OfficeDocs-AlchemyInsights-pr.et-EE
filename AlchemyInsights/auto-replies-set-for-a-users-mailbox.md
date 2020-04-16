---
title: Postkasti automaatvastuste määramine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: aeeb2e1e76fe602d2767b422797452fd1155fdd5
ms.sourcegitcommit: fdfd41c2bfb2d45003b3906e6469377384a91cb5
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2020
ms.locfileid: "43509490"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Kasutaja postkasti automaatvastuste määramine

**1. meetod**

1. Logige sisse Office 365 portaali.

2. Avage suvand **Kasutajad > Aktiivsed kasutajad** (või **Rühmad > Ühispostkastid**, kui määrate selle ühispostkastile).

3. Valige kasutaja, kellel on Microsoft Exchange’i postkast.

4. Avage parempoolses hüpikmenüüd **Meilisätted > Automaatvastused** (kui see on ühispostkast, klõpsake lihtsalt hüpikmenüüs suvandit **Automaatvastused**).

**2. meetod**

1. Logige administraatori identimisteavet kasutades sisse Office 365 haldusportaali.

2. Laiendage suvandit **Halduskeskused** ja seejärel klõpsake suvandit **Exchange**.

3. Klõpsake paremas ülanurgas olevat pilti, klõpsake suvandit **Teine kasutaja** ja seejärel valige kasutaja postkast, mida soovite muuta.

4. Valige vasakus servas valik **Suvandid**, klõpsake suvandit **Meilide korraldamine** ja klõpsake seejärel suvandit **Automaatvastused.**

**3. meetod**

Käivitage Exchange Online PowerShellis järgmine cmdlet-käsk:

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

Selle cmdlet-käsu kohta leiate lisateavet artiklist [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
