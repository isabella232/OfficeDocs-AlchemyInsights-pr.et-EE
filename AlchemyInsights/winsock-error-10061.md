---
title: 1554 Winsock tõrge 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766165"
---
# <a name="winsock-error-10061"></a>Winsock tõrge 10061

See tõrkekood tähendab, et Microsoft ei saa luua TCP pesa (ühendus) Target hosti. Selle tõrke kõige tõenäolisem põhjus on tulemüüri konfiguratsiooniga seotud probleem. Probleemi lahendamiseks kontrollige järgmisi sätteid.

- Kontrollige oma tulemüüri konfiguratsiooni teavet [Microsoft 365 URL-id ja IP-aadresside vahemikud](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Kui tõrge on seotud Exchange Online Protection (EOP), peaks olema varem teatatud muutus [Exchange Online Protection IP-aadressid](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Veenduge, et teie Interneti-teenuse pakkuja (ISP) ei blokeeri porti.

- Kontrollige oma konnektorite nutikat hosti ja sihtserveri sätteid.

Pange tähele, et Microsoft 365 ei blokeeri *sissetulevad* ühendused sel viisil.
