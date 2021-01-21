---
title: Märkide eluea konfigureerimine ja laiendamine
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916823"
---
# <a name="configure-and-extend-token-lifetimes"></a>Märkide eluea konfigureerimine ja laiendamine

Saate määrata Microsoft Identity Platformi poolt välja antud Accessi, SAML või ID-tõendi kestuse. Saate määrata märkide eluea kõigi oma asutuse rakenduste jaoks, mitme rentniku (mitme organisatsiooni) rakenduse jaoks või ettevõtte teatud teenuse põhiosa jaoks. Lisateavet leiate teemast [Konfigureeritav sümboolne kasutusaeg](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

Näiteid leiate teemast [märkide eluea konfigureerimine](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).

Lisateavet selle kohta, kuidas konfigureerida Azure Active Directory B2C (Azure AD B2C) loa kehtivust ja ühilduvust, leiate teemast [märkide konfigureerimine Azure Active DIRECTORY B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).

[Azure Active DIRECTORY B2C seansi käitumise konfigureerimine](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) selles artiklis kirjeldatakse AZURE ad B2C kasutatavaid ühekordse SISSELOGIMISE (SSO) meetodeid ja see aitab teil poliitika konfigureerimisel valida kõige sobivama SSO meetodi.

**Kui kaua märgid kestavad? Kui kaua need kehtivad?**

Märkide eluiga on 1 tund ja seansi kasutusaeg on 24 tundi. See tähendab, et kui 24 tunni jooksul pole taotlusi esitatud, peate enne uue loa taotlemist uuesti sisse logima.

> [!NOTE]
> Pärast 30. mail 2020 ei saa uut rentnikku kasutada konfigureeritav sümboolne eluaegset poliitikat seansi ja märkide värskendamise konfigureerimiseks. Aegumine juhtub mitme kuu jooksul pärast seda, mis tähendab, et me lõpetame olemasoleva seansi austamise ja märkide värskendamise. Saate ikkagi konfigureerida juurdepääsu turbelubade eluea pärast selle möödumist.






