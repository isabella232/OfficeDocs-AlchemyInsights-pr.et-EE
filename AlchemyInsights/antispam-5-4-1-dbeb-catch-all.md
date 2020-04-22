---
title: Rämpspostitõrje 5.4.1 DBEB saagi-kõik
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707907"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Fix kohaletoimetamise probleemid tõrkekood 550 5.4.1 relee juurdepääs keelatud

See probleem ilmneb siis [, kui kontrollida, kas e-posti aadress on kehtiv vältida bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) sisestamisel Microsoft Network. Proovige järgmist:

1. Tehke kindlaks, kas probleem on seotud kogu domeeni või ühe e-posti aadress:
    - Kogu Domeen: mõnikord peab Domeen olema sünkroonitud; Proovige [domeeni sisemine ja seejärel tagasi autoriteetne](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Üks e-posti aadress: mõnikord tuleb aadress sünkroonida; SMTP puhverserveri aadressi muutmine ja seejärel uuesti muutmine aitab.
2. Tehke kindlaks, kas probleem on seotud rühma või ühiskausta. Mõne objektitüübi puhul võib osutuda vajalikuks objektide käsitsi loomine Azure Active Directorys.

Kui vajate täiendavat abi, siis avage tugiteenuse pilet ja määrake probleemi ulatus (sh teie poolt saatva objekti tüüp), et saaksime teid paremini aidata.