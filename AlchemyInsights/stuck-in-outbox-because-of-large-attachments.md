---
title: Takerdunud väljundkasti suurte manuste tõttu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241248"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Sõnumite parandamine, mis on väljundkaustas kinni

Soovitame alustada, käivitades stsenaariumi ["Mul on probleeme saatmine, vastuvõtmine või leidmine"](https://aka.ms/SaRA-OutlookSendReceive) [Microsofti toe ja taastamise abimees](https://diagnostics.office.com/#/) tööriista.

Kui sõnum jääb teie väljundkaustas kinni, on kõige tõenäolisem põhjus suur manus või suvand "saada kohe, kui see on ühendatud" pole lubatud.

**Eemaldage suur manus**

1. Outlookis valige **saatmise/vastuvõtu** > **töö ühenduseta**. 
2. Valige navigeerimispaanil suvand **Väljundboks**. Siit saate: 
    - Kustutage sõnum (valige see ja seejärel valige **Kustuta**).
    - Lohistage sõnum mustandite kausta, topeltklõpsake selle avamiseks ja manuse eemaldamiseks valige see ja seejärel valige **Kustuta**).
3. Kui kuvatakse tõrketeade, mis ütleb, et Outlook proovib sõnumit edastada, sulgege Outlook. Väljumiseks võib kuluda mõni hetk. Kui Outlook ei sulge, vajutage klahvikombinatsiooni CTRL + ALT + DELETE ja valige **Käivita Tegumihaldur**. Valige Tegumihalduris vahekaart **protsessid** , kerige allapoole Outlook. exe ja valige **Lõpeta protsess**.
4. Pärast Outlooki sulgemist taaskäivitage see ja korrake juhiseid 2 ja 3. 
5. Pärast manuse eemaldamist klõpsake nuppu **Saada/võta vastu** > **Tööta ühenduseta** , et jätkata töötamist ühendusega. 

Sõnumid jäävad ka väljundkasti, kui klõpsate nuppu **saada**, kuid te ei ole ühendatud. Klõpsake nuppu **Saada/võta vastu** ja vaadake **ühenduseta töö** nuppu. Kui see on sinine, siis sa oled lahutatud. Klõpsake seda ühendamiseks (nupp muutub valgeks) ja klõpsake **saada kõik**.
 
**Luba saatmine kohe, kui see on ühendatud**
 
1. Klõpsake menüü Fail käsku **Suvandid**.

2. Klõpsake dialoogiboksis Outlooki suvandid nuppu **Täpsemalt**.

3. Klõpsake jaotises saatmise ja vastuvõtu lubamiseks **Saada kohe, kui**see on ühendatud. Klõpsake nuppu **OK**.
 
Täielikud üksikasjad leiate teemast:
- [Video: saata või kustutada ummikus e-posti](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [E-posti jääb kausta saatmiseks kuni te käsitsi algatada saatmise/vastuvõtu toiming Outlookis](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
