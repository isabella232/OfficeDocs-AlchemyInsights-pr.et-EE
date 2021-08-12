---
title: Klassikalise juursaidi vahetamine modernsaidiga
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 7209595f5cda9b31e53241d9d5696fa584ff5e5ab3d237aae28542bf7aec9398
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940815"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Klassikalise juursaidi vahetamine modernsaidiga

Kui teie keskkond oli häälestatud enne 2019. aasta aprilli, saate juursaidi microsoft PowerShelli abil muuta modernsaidiks.

- Kui teil on muu sait, mida soovite juursaidina kasutada, saate juursaidi asendada [(vahetada).](https://docs.microsoft.com/sharepoint/modern-root-site) 
    - Kasutage [invoke-SPOSiteSwapi,](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) et vahetada saidi asukoht teise saidiga algse saidi arhiivimise ajal. Saadaval nii meeskonnatöö saidi (pole rühmaga ühendatud) kui ka suhtlussaidi jaoks. 

- Peagi tutvustatakse täiendavaid võimalusi, mis võimaldavad teil saidi sisu edasi kasutada, kuid teisendada olemasoleva saidi suhtlussaidiks. 
>[!Important]
>Need võimalused on järk-järgult välja tõstnud. Jätkake sõnumikeskuse värskenduste otsimist. 

## <a name="known-issues-with-swapping-sites"></a>Teadaolevad probleemid saitide vahetamisega

- Sihtsaidil võib lühikese aja jooksul tagastada tõrke "ei leitud" (HTTP 404).
- Otsinguregistri värskendamiseks tuleb sisu uuesti joonistada. Käsitsi pole vaja teha – seda tehakse automaatselt.
- Kõik,mis sõltub "staatilistest" linkidest (nt failisünkroonimine OneNote failid), tuleb käsitsi parandada.
- Kui lähtesaidiks oli organisatsiooni uudiste sait, värskendage URL-i. Hankige kõigi organisatsiooni uudistesaitide loend.
- Project Võimalik, et serverisaidid tuleb valideerida, et veenduda, et need on endiselt õigesti seostatud.
