---
title: Kaasaegne sait kui root sait
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2e2bb02b9dbaf7f8ede0b4c5ba8c8f29453309cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054698"
---
# <a name="modern-site-as-root-site"></a>Kaasaegne sait root sait

Oleme hakanud rollout uus funktsioon, mis võimaldab teil [vahetada oma klassikalise saidi root saidi kaasaegse saidi](https://docs.microsoft.com/sharepoint/modern-root-site). Kasutage [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) vahetada saidi asukoha teise saidi arhiveerimise algse saidi. Saadaval nii meeskonnatöö sait (ei ole ühendatud rühma) ja side saidi.

>[!Important]
> Ärge kustutage oma klassikalist juursaiti, et luua kaasaegne Kommunikatsioonisait. Microsoft ei toeta seda. Juursaidi kustutamisel tehakse kõik SharePointi saidid teie organisatsioonis kättesaamatuks kõigile kasutajatele, kuni saate saidi taastada või luua uue saidi samas URL-is. Edastame selle funktsiooni sõnumikeskuse kaudu. Peaksite ootama, et funktsioon oleks teie rentnikus peagi sisse lülitatud.

## <a name="known-issues-with-swapping-sites"></a>Teadaolevad probleemid vahetamise saidid
- Target sait võib tagastada "ei leitud" (HTTP 404) tõrge lühikese aja jooksul.
- Otsinguindeksi värskendamiseks tuleb sisu uuesti värskendada. Siin ei ole manuaalset sammu vaja, seda tehakse automaatselt.
- Midagi sõltub "staatiline" linke (nt faili sünkroonimine ja OneNote faile) tuleb käsitsi parandada.
- Project Serveri saidid võib olla vaja valideerida, et tagada, et need on endiselt õigesti seotud. 
