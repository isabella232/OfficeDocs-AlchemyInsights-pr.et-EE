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
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698858"
---
# <a name="winsock-error-10061"></a>Winsocki tõrge 10061

See tõrkekood tähendab seda, et Microsoft ei suutnud luua Target hostiga TCP-liidest (ühendust). Selle tõrke kõige tõenäolisem põhjus on probleem tulemüüri konfiguratsiooniga. Probleemi lahendamiseks vaadake järgmisi sätteid.

- Tulemüüri konfiguratsiooni kinnitamine [Microsoft 365 URL-ide ja IP-aadresside vahemikega](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges) seotud teabega

- Kui tõrkeks on Exchange Online ' i kaitse (EOP), oleks pidanud eelnevalt olema teatatud [Exchange Online ' i kaitse IP-aadresside](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)muutmisest.

- Veenduge, et teie Interneti-teenuse pakkuja (ISP) ei blokeeriks porti.

- Kontrollige, kas konnektorid on nutikad Host ja Target serveri sätted.

Pange tähele, et Microsoft 365 ei blokeeri sel viisil *sissetulevaid* ühendusi.
