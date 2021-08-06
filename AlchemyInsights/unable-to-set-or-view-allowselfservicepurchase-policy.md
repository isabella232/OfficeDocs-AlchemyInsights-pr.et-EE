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
ms.openlocfilehash: 255dbe35b808b3fe6b5707779251bf3f4a7e1c269c8b6f0ac2cb43ca03c469e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020188"
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

