---
title: Kasutaja postkasti automaatvastuste määramine
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
ms.openlocfilehash: e3cc01298c10fd3ba21327a7fb5cc5396d0ad74d
ms.sourcegitcommit: 23e5b94f1758bfe202008384e300b81816975375
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/14/2020
ms.locfileid: "43506456"
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

    Set-MailboxAutoReplyConfiguration

Selle cmdlet-käsu kohta leiate lisateavet artiklist [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
