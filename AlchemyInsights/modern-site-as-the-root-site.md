---
title: Modernne sait juursaidina
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
ms.openlocfilehash: a0f48dc79b51168c9cc045078ad8fc7d668343c7
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327598"
---
# <a name="modern-site-as-root-site"></a>Modernne sait juursaidina

Oleme alustanud uue funktsiooni väljajuurimist, mis võimaldab teil klassikalise saidi juursaidi [modernsaidiga vahetada.](https://docs.microsoft.com/sharepoint/modern-root-site) Kasutage [invoke-SPOSiteSwapi](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) saidi asukoha vahetamiseks mõne muu saidiga algse saidi arhiivimise ajal. Saadaval nii meeskonnatöö saidi (pole rühmaga ühendatud) kui ka suhtlussaidi jaoks.

**Tähtis.** Modernse suhtlussaidi loomiseks ärge kustutage klassikalist juursaidi. Microsoft ei toeta seda. Juursaidi kustutamisel ei pääse SharePoint kõik teie ettevõtte saidid kõigile kasutajatele, kuni taastate saidi või loote samal URL-il uue saidi. Edastame selle funktsiooni sõnumikeskuse kaudu. Peaksite eeldama, et funktsioon on peagi teie rentnikus sisse lülitatud.

## <a name="known-issues-with-swapping-sites"></a>Teadaolevad probleemid saitide vahetamisega
- Sihtsaidil võib lühikese aja jooksul tagastada tõrke "ei leitud" (HTTP 404).
- Otsinguregistri värskendamiseks tuleb sisu uuesti joonistada. Siin pole vaja käsitsi teha, see tehakse automaatselt.
- Kõik, mis sõltub "staatilistest" linkidest (nt failisünkroonimine OneNote failidest), tuleb käsitsi parandada.
- Project Võimalik, et serverisaidid tuleb valideerida, et veenduda, et need on endiselt õigesti seostatud. 
