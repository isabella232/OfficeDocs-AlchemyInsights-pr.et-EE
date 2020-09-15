---
title: Kaasaegne sait juure saidina
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666866"
---
# <a name="modern-site-as-root-site"></a>Kaasaegne sait juure saidina

Oleme alustanud uue funktsiooni väljatöötamist, mis võimaldab teil [vahetada oma klassikalist saidi juurt modernse](https://docs.microsoft.com/sharepoint/modern-root-site)saidiga. Kasutage [SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) , et vahetada saidi asukoht teise saidiga, arhiivides algse saidi. Saadaval nii meeskonnatöö saidi jaoks (pole rühmaga ühendatud) kui ka kommunikatsiooni saidil.

>[!Important]
> Ärge kustutage oma klassikalist juurt, et luua kaasaegne kommunikatsiooni sait. Microsoft ei toeta seda. Juurte saidi kustutamine muudab kõik teie organisatsioonis olevad SharePointi saidid kõigile kasutajatele juurdepääsetavaks, kuni taastate saidi või loote sama URL-is uue saidi. Edastame selle funktsiooni teateriba kaudu. Peate eeldama, et funktsioon on rentniku jaoks peagi sisse lülitatud.

## <a name="known-issues-with-swapping-sites"></a>Saidid vahetamise teadaolevad probleemid
- Sihtkaust võib tagastada lühikese aja jooksul tõrketeate "ei leitud" (HTTP 404).
- Otsingu indeksi värskendamiseks tuleb sisu uuesti analüüsida. Siin pole käsitsi vajalikku juhiseid, seda tehakse automaatselt.
- Midagi, mis sõltub staatilisest lingist (nt failide sünkroonimine ja OneNote ' i failid), tuleb käsitsi parandada.
- Võimalik, et Project Serveri saidid peavad olema valideeritud, et veenduda, et need on endiselt õigesti seotud. 
