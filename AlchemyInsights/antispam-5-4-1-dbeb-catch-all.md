---
title: AntiSpam 5.4.1 DBEB Catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717357"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Kohaletoimetamisega seotud probleemide lahendamine tõrkekood 550 5.4.1 relee juurdepääs on keelatud

See probleem ilmneb siis [, kui kontrollitakse, kas e-posti aadress kehtib bouncebacks takistamiseks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) Microsofti võrku sisenemisel. Proovige teha järgmist.

1. Määratlege, kas probleem on seotud kogu domeeni või ühe meiliaadressiga.
    - Kogu Domeen: mõnikord peab domeeni sünkroonima; Proovige [määrata Domeen asutusesiseseks ja seejärel tagasi autoriteetseks](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Üks meiliaadress: mõnikord tuleb aadress sünkroonida; SMTP-puhverserveri aadressi muutmine ja selle uuesti muutmine võib aidata.
2. Määratlege, kas probleem on seotud mõne rühma või Ühiskaustaga. Mõne objekti tüübi korral võib olla vaja, et Azure Active Directorys on objektid käsitsi loodud.

Kui vajate täiendavat abi, avage klienditoe pilet ja määrake probleemi ulatus (sh objekti tüüp), et saaksime teid paremini aidata.