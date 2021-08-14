---
title: Kustutatud rühma Microsoft 365 taastamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: 6262ca04335c355fb4de41a9e1d854b666f47e10321a843717d6eb951c46cafd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959022"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Kustutatud rühma Microsoft 365 taastamine

Kustutatud rühma või Microsoft 365 saate taastada Microsoft Teams 30 päeva jooksul pärast kustutamist.

1. Avage [Microsoft 365 halduskeskus,](https://aka.ms/RestoreDeletedGroup) et logida sisse kustutatud rühmade ja töörühmade loendisse.

    **Märkus.** Logige sisse rentnikuadministraatori või rühmaadministraatori rollile määratud kontoga.

1. Valige taastamiseks Microsoft 365/Teams ja klõpsake nuppu **Taasta rühm**.

    Kui rühma ei saa vastuoluliste SMTP-aadresside tõttu taastada, kasutage konflikti põhjustava objekti leidmiseks ja SMTP-aadressi eemaldamiseks järgmist käsku.

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Märkus.** Mõnel juhul võib rühma ja kõigi selle andmete taastamine võtta kuni 24 tundi.

    Lisateavet powerShelli abil rühmade taastamise kohta leiate teemast Kustutatud rühma [Microsoft 365 taastamine.](https://go.microsoft.com/fwlink/?linkid=867802)