---
title: SharePoint Online ' i ahendamine
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931222"
---
# <a name="sharepoint-online-throttling"></a>SharePoint Online ' i ahendamine

**Oluline**: paljud SharePoint Online ' i ja OneDrive kliendid käivitada Business kriitilised rakendused teenuse, mis töötavad taustal. Nende hulka kuuluvad sisu migratsioon, andmete kadu vältimine (DLP) ja backup lahendused. Nendel enneolematul ajal me võtame meetmeid, et tagada SharePoint Online ' i ja OneDrive teenused on väga kättesaadav ja usaldusväärne oma kasutajatele, kes sõltuvad teenuse rohkem kui kunagi varem kaugtöö stsenaariume.

Selle eesmärgi toetuseks oleme rakendanud ranget ahendamise piiranguid taustal olevatele rakendustele (migratsioon, DLP ja backup lahendused) tööpäeval päeva jooksul. Te peaksite ootama, et need rakendused saavutavad nende aegade jooksul väga piiratud läbilaskevõime. Aga, õhtuti ja nädalavahetusel tundi piirkonna, teenus on valmis töötlema oluliselt suurem hulk taotlusi taustal apps.

**503 server on hõivatud tõrge**

Kasutajad võivad saada 503 server on hõivatud tõrge katsel navigeerida SharePointi või OneDrive saidid. 

See tõrge võib põhjustada ahendamine jooksul SharePointi teenus. SharePoint Online ' i kasutab ahendamine optimaalse jõudluse ja töökindluse SharePoint Online Service. Ahendamine piirab kasutajate toimingute või samaaegsete kõnede (skripti või koodi) arvu, et vältida ressursside ülekasutamist. 

Ahendamise kohta lisateabe saamiseks [Vältige saada ahendatud või blokeeritud SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

Kui arvate, et see tõrge ei ole seotud ahendamine, saate kontrollida, kas on aktiivne hooldus esineb teie rentniku navigeerides [sõnumikeskus](https://portal.office.com/adminportal/home#/MessageCenter).

 Lõpuks, veenduge, et külastate [teenuse tervis](https://portal.office.com/adminportal/home#/servicehealth) lehte, et kontrollida mis tahes teateid/intsidente, mis võivad tekkida.

