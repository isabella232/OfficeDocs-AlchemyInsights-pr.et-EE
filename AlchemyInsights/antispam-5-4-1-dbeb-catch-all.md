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
ms.openlocfilehash: e0e9b4fec0615943227f40043aeed842e8ee556c5916a59f65e79ce121ec9547
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932273"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Tõrkekoodi 550 5.4.1 edastamisega seotud probleemide lahendamine

See probleem ilmneb [siis, kui kontrollite, kas](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) meiliaadress on kehtiv, et vältida Microsofti võrku sisenemisel tagasipöördumiseid. Proovige järgmist.

1. Tehke kindlaks, kas probleem on seotud terve domeeni või ühe meiliaadressiga.
    - Kogu domeen. Mõnikord tuleb domeen sünkroonida; proovige [määrata domeeniks Internal (Sisemine) ja seejärel valige uuesti Authoritative (Autoriteetne).](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)
    - Ühekordne meiliaadress: mõnikord tuleb aadress sünkroonida; Smtp-puhverserveri aadressi muutmine ja selle tagasi muutmine võib aidata.
2. Tehke kindlaks, kas probleem on seotud rühma või avaliku kaustaga. Mõne objektitüübi puhul tuleb objektid võib-olla käsitsi luua Azure Active Directory.

Kui vajate täiendavat abi, avage tugiteenuste pilet ja määrake probleemi ulatus (sh selle objekti tüüp, mida saadate), et saaksime teid paremini aidata.