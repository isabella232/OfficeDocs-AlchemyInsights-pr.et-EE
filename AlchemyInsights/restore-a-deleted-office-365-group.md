---
title: Kustutatud Microsoft 365 rühma taastamine
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
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597439"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Kustutatud Microsoft 365 rühma taastamine

Kustutatud Microsoft 365 rühma või Microsoft Teamsi saate taastada 30 päeva jooksul pärast kustutamist.

1. Logige sisse [Microsoft 365 halduskeskusesse](https://aka.ms/RestoreDeletedGroup) ja loetlege kustutatud rühmad ja töörühmad.

    **Märkus.** Logige sisse rentnikuadministraatori või rühmaadministraatori rollile määratud kontoga.

1. Valige taastamiseks kustutatud Microsoft 365 rühm/Teams ja klõpsake nuppu **Taasta rühm**.

    Kui rühma ei saa vastuoluliste SMTP-aadresside tõttu taastada, kasutage konflikti põhjustava objekti leidmiseks ja SMTP-aadressi eemaldamiseks järgmist käsku.

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Märkus.** Mõnel juhul võib rühma ja kõigi selle andmete taastamine võtta kuni 24 tundi.

    Lisateavet powerShelli abil rühmade taastamise kohta leiate teemast Kustutatud [Microsoft 365 rühma taastamine.](https://go.microsoft.com/fwlink/?linkid=867802)