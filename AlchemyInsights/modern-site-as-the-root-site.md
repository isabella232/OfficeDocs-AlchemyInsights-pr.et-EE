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
ms.openlocfilehash: b42cf276a76547584c8cfd87b5a28f31d51ea7f8ca56621b22aeef01e4613ce6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000383"
---
# <a name="modern-site-as-root-site"></a>Modernne sait juursaidina

Oleme alustanud uue funktsiooni väljajuurimist, mis võimaldab teil klassikalise saidi juursaidi [modernsaidiga vahetada.](https://docs.microsoft.com/sharepoint/modern-root-site) Kasutage [invoke-SPOSiteSwapi,](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) et vahetada saidi asukoht teise saidiga algse saidi arhiivimise ajal. Saadaval nii meeskonnatöö saidi (pole rühmaga ühendatud) kui ka suhtlussaidi jaoks.

>[!Important]
> Modernse suhtlussaidi loomiseks ärge kustutage klassikalist juursaidi. Microsoft ei toeta seda. Juursaidi kustutamisel ei pääse SharePoint kõik teie ettevõtte saidid kõigile kasutajatele, kuni taastate saidi või loote samal URL-il uue saidi. Edastame selle funktsiooni sõnumikeskuse kaudu. Peaksite eeldama, et funktsioon on peagi teie rentnikus sisse lülitatud.

## <a name="known-issues-with-swapping-sites"></a>Teadaolevad probleemid saitide vahetamisega
- Sihtsaidil võib lühikese aja jooksul tagastada tõrke "ei leitud" (HTTP 404).
- Otsinguregistri värskendamiseks tuleb sisu uuesti joonistada. Siin pole vaja käsitsi teha, see tehakse automaatselt.
- Kõik,mis sõltub "staatilistest" linkidest (nt failisünkroonimine OneNote failid), tuleb käsitsi parandada.
- Project Võimalik, et serverisaidid tuleb valideerida, et veenduda, et need on endiselt õigesti seostatud. 
