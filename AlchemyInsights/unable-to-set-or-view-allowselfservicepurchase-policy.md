---
title: AllowSelfServicePurchase'i poliitikat ei saa seada ega vaadata
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
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826087"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>AllowSelfServicePurchase'i poliitikat ei saa seada ega vaadata

Kui proovite seada või vaadata AllowSelfServicePurchase'i poliitikat, kuvatakse järgmine tõrketeade:

*HandleError : Tootepoliitika toomine poliitikaga "AllowSelfServicePurchase", ErrorMessage nurjus – aluseks olev ühendus suleti: saatmisel ilmnes ootamatu tõrge.*

Põhjuseks võib olla transpordikihi turbe (TLS) vanem versioon. MSCommerce'i teenuse ühendamiseks peate kasutama TLS 1.2 või suuremat versiooni.  

TLS-protokolli lubamiseks/1.2 lubamiseks,kinnitamiseks ja uuesti proovimiseks proovige järgmisi juhiseid.
 1. Sisestage PowerShelli käsuviibale (PS C) järgmine käsk, et \) määrata TLS-protokolliks versioon 1.2.

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Kontrollige, kas TLS-protokoll(id) on kasutusel, järgmise käsuga:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Vajaduse korral saate uuesti käivitada käsud Too või Värskenda.

