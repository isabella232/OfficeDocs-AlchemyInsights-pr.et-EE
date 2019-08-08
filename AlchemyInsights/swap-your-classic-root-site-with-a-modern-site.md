---
title: Vaheta klassikaline juursait mis kaasaegne veebilehekülg
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "2579"
- "9000687"
ms.openlocfilehash: dad7d7a52222dc09aea532714a93ca89c0d9ae19
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/07/2019
ms.locfileid: "36245963"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Vaheta klassikaline juursait mis kaasaegne veebilehekülg

Kui teie keskkonnas oli enne aprilli 2019, saate muuta oma juursait kaasaegne veebilehekülg Microsoft PowerShelli abil:

- Kui teil on mõni muu sait, mida soovite kasutada oma juursait, saate asendada (swap) juur saidi see. 
    - Vahetada asukoht teise saidiga algse saidi arhiveerimise ajal kasutada [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) . Saadaval Team Site (ühendatud rühma) ja teatise ala. 

- Võetakse kasutusele täiendavad võimalused kiiresti, mis lubab kasutada saidi sisu, kuid muuta olemasoleva saidi teatis saidile. 
>[!Important]
>Need võimed on rullitakse järk-järgult. Edasi kontrollige värskendusi Office 365 sõnumikeskus. 

## <a name="known-issues-with-swapping-sites"></a>Tuntud probleemid tootega vahetada saidid

- Sihtsaidi tagastab "ei leitud" viga (HTTP 404) lühikest aega.
- Sisu tuleb analüüsitakse uuesti värskendada otsinguregistrisse. Ei ole vaja käsitsi sammu - seda tehakse automaatselt.
- Midagi sõltub "staatiline" lingid (nt faili sünkroonimine ja OneNote) pead käsitsi korrigeerida.
- Kui allika ala oli organisatsiooni uudistesaidi, muudetud URL.Saada kõik organisatsiooni Uudised kohad.
- Project Serveri saidid võib tekkida vajadus tagada, et need on ikka seotud õigesti kinnitada.





