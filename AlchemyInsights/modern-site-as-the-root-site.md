---
title: Kaasaegne saidi juursait
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 260048db6c439183da8e0bb0c2dfa3c7475fca79
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/09/2019
ms.locfileid: "36269372"
---
# <a name="modern-site-as-root-site"></a>Kaasaegne saidi juur

Oleme hakanud levikuga uus funktsioon, mis võimaldab teil vahetada klassikaline saidi juursait mis kaasaegne veebilehekülg. Vahetada asukoht teise saidiga algse saidi arhiveerimise ajal kasutada [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) . Saadaval Team Site (ühendatud rühma) ja teatise ala. 

>[!Important]
> Ärge kustutage oma klassikaline juursait kaasaegsed side saidi loomiseks. See ei toeta Microsoft. Kustutamine juursait teeb kõik SharePointi saidid teie organisatsiooni juurdepääs kõigile kasutajatele, kuni taastamist või luua uue saidi sama URL. Me suhtlemine selle funktsiooni kaudu sõnumikeskus. Teil tuleb arvestada funktsioon olema sisse lülitatud teie rentniku varsti.

## <a name="known-issues-with-swapping-sites"></a>Tuntud probleemid tootega vahetada saidid
- Sihtsaidi tagastab "ei leitud" viga (HTTP 404) lühikest aega.
- Sisu tuleb analüüsitakse uuesti värskendada otsinguregistrisse. Ei mingit käsitsi sammu vajalike, seda tehakse automaatselt.
- Midagi sõltub "staatiline" lingid (nt faili sünkroonimine ja OneNote) pead käsitsi korrigeerida.
- Project Serveri saidid võib tekkida vajadus tagada, et need on ikka seotud õigesti kinnitada. 
