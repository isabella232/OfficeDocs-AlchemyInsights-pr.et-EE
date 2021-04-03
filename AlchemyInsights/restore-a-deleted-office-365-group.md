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
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505682"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Kustutatud Microsoft 365 rühma taastamine

Kustutatud Microsoft 365 rühma või Microsoft Teamsi saate taastada 30 päeva jooksul pärast kustutamist.

1. Microsoft 365 halduskeskusesse sisselogimiseks ning kustutatud rühmade ja töörühmade loendi vaatamiseks avage [Microsoft 365 halduskeskus.](https://aka.ms/RestoreDeletedGroup)

    **Märkus.** Logige sisse rentnikuadministraatori või rühmaadministraatori rollile määratud kontoga.

1. Valige taastamiseks kustutatud Microsoft 365 rühm/Teams ja klõpsake nuppu **Taasta rühm**.

    Kui rühma ei saa vastuoluliste SMTP-aadresside tõttu taastada, kasutage konflikti põhjustava objekti leidmiseks ja SMTP-aadressi eemaldamiseks järgmist käsku.

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Märkus.** Mõnel juhul võib rühma ja kõigi selle andmete taastamine võtta kuni 24 tundi.

    Lisateavet powerShelli abil rühmade taastamise kohta leiate teemast Kustutatud [Microsoft 365 rühma taastamine.](https://go.microsoft.com/fwlink/?linkid=867802)