---
title: Ei saa seada või vaadata AllowSelfServicePurchase poliitika
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158557"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Ei saa seada või vaadata AllowSelfServicePurchase poliitika

Kui proovite seada või vaadata AllowSelfServicePurchase poliitika, kuvatakse järgmine tõrketeade:

*HandleError: tootepoliitika hankimine poliitika ID ' AllowSelfServicePurchase ', ErrorMessage-aluseks olev ühendus suleti: saatmisel ilmnes ootamatu tõrge.*

See võib olla tingitud vanem versioon transpordikihi turbe (TLS). MSCommerce teenuse ühendamiseks peate kasutama TLS 1,2 või uuem.  

Proovige/seadke TLS-i protokoll 1,2, kontrollige ja proovige järgmisi samme.
 1. PowerShelli Käsuviip (PS C:\) sisestage järgmine käsk, et määrata TLS-i protokolli versioon 1,2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Veenduge, et TLS-protokoll (ID) kasutusel, järgmine käsk:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Proovige vajadusel käsku Võta või uuenda.

