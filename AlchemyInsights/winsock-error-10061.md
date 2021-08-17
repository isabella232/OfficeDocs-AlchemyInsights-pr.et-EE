---
title: 1554 Winsocki tõrge 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083226"
---
# <a name="winsock-error-10061"></a>Winsocki tõrge 10061

See tõrkekood tähendab, et Microsoft ei saanud sihthostiga TCP-soklit (ühendust) luua. Selle tõrke kõige tõenäolisem põhjus on probleem tulemüüri konfiguratsioonis. Probleemi lahendamiseks kontrollige järgmisi sätteid.

- Kontrollige tulemüüri konfiguratsiooni Microsoft 365 [URL-ide ja IP-aadresside vahemike teabega](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Kui tõrge on seotud Exchange Online'i kaitseteenus (EOP), oleks teid eelnevalt pidanud Exchange Online'i kaitseteenus [muudatusest.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

- Veenduge, et teie Interneti-teenuse pakkuja (ISP) ei blokeeriks porti.

- Veenduge, et teie konnektorites on nutika hosti ja sihtserveri sätted.

Arvestage, Microsoft 365 ei blokeeri *sissetulevaid* ühendusi sel viisil.
