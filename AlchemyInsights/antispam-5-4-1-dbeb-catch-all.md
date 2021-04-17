---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821443"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Tõrkekoodi 550 5.4.1 edastamisega seotud probleemide lahendamine

See probleem ilmneb [siis, kui kontrollite, kas](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) meiliaadress on kehtiv, et vältida Microsofti võrku sisenemisel tagasipöördumiseid. Proovige järgmist.

1. Tehke kindlaks, kas probleem on seotud terve domeeni või ühe meiliaadressiga.
    - Kogu domeen. Mõnikord tuleb domeen sünkroonida; proovige [määrata domeeniks Internal (Sisemine) ja seejärel valige uuesti Authoritative (Autoriteetne).](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)
    - Ühekordne meiliaadress: mõnikord tuleb aadress sünkroonida; Smtp-puhverserveri aadressi muutmine ja selle tagasi muutmine võib aidata.
2. Tehke kindlaks, kas probleem on seotud rühma või avaliku kaustaga. Mõne objektitüübi puhul tuleb objektid azure Active Directorys käsitsi luua.

Kui vajate täiendavat abi, avage tugiteenuste pilet ja määrake probleemi ulatus (sh selle objekti tüüp, mida saadate), et saaksime teid paremini aidata.