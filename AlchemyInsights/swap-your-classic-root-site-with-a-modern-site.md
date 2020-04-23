---
title: Vaheta oma Classic root saidi kaasaegne sait
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741540"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Vaheta oma Classic root saidi kaasaegne sait

Kui teie keskkond on seadistatud enne aprill 2019, saate muuta oma juursaiti kaasaegne sait, kasutades Microsoft PowerShelli:

- Kui teil on erinev sait, mida soovite kasutada oma root saidi, saate asendada [(swap) root saidi](https://docs.microsoft.com/sharepoint/modern-root-site) koos sellega. 
    - Kasutage [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) vahetada saidi asukoha teise saidi arhiveerimise algse saidi. Saadaval nii meeskonnatöö sait (ei ole ühendatud rühma) ja side saidi. 

- Varsti võetakse kasutusele täiendavad võimalused, mis võimaldavad teil saidi sisu kasutada, kuid teisendage olemasolev sait suhtlussaidile. 
>[!Important]
>Need võimed tehakse järk-järgult. Jätkake teadete keskuse värskenduste kontrollimiseks. 

## <a name="known-issues-with-swapping-sites"></a>Teadaolevad probleemid vahetamise saidid

- Target sait võib tagastada "ei leitud" (HTTP 404) tõrge lühikese aja jooksul.
- Otsinguindeksi värskendamiseks tuleb sisu uuesti värskendada. Ei ole manuaalset sammu vaja-seda tehakse automaatselt.
- Midagi sõltub "staatiline" linke (nt faili sünkroonimine ja OneNote faile) tuleb käsitsi parandada.
- Kui Lähtesait oli organisatsiooni uudistesait, värskendage URL-i.Saate hankida kõigi organisatsiooniuudiste saitide loendi.
- Project Serveri saidid võib olla vaja valideerida, et tagada, et need on endiselt õigesti seotud.
