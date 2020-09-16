---
title: AllowSelfServicePurchase poliitikat ei saa seada ega vaadata
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
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735195"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>AllowSelfServicePurchase poliitikat ei saa seada ega vaadata

Kui proovite määrata või vaadata AllowSelfServicePurchase poliitikat, kuvatakse järgmine tõrketeade:

*HandleError: PolicyId ' AllowSelfServicePurchase ', sündmustelogist-ga tootepoliitika toomine nurjus: saatmisel ilmnes ootamatu tõrge.*

See võib olla tingitud transpordikihi turbe (TLS) varasemast versioonist. MSCommerce teenusega ühenduse loomiseks peate kasutama TLS 1,2 või uuemat versiooni.  

Toimige järgmiselt, et lubada/seadistada TLS-protokoll 1,2, kinnitada ja uuesti proovida.
 1. PowerShelli käsureal (PS C: \) Sisestage järgmine KÄSK TLS-protokolli versioonile 1,2 määramiseks tehke järgmist.

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Kontrollige, kas TLS-protokoll (ID) on kasutusel, ja kasutage järgmist käsku.

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Proovige käske Too või Värskenda uuesti vastavalt vajadusele.

