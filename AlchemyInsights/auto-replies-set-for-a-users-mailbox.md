---
title: Postkasti automaatvastuste määramine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 60af581e7fe508ab9644a53873bcd551b3aacff1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820930"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Kasutaja postkasti automaatvastuste määramine

**1. meetod**

1. Logige sisse Microsoft 365 portaali.

2. Avage suvand **Kasutajad > Aktiivsed kasutajad** (või **Rühmad > Ühispostkastid**, kui määrate selle ühispostkastile).

3. Valige kasutaja, kellel on Microsoft Exchange’i postkast.

4. Avage parempoolses hüpikmenüüd **Meilisätted > Automaatvastused** (kui see on ühispostkast, klõpsake lihtsalt hüpikmenüüs suvandit **Automaatvastused**).

**2. meetod**

1. Logige administraatori identimisteavet kasutades sisse Microsoft 365 haldusportaali.

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
