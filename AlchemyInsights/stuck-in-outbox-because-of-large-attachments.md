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
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232626"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Sõnumite parandamine, mis on väljundkaustas kinni

Soovitame alustada, käivitades stsenaariumi ["Mul on probleeme saatmine, vastuvõtmine või leidmine"](https://aka.ms/SaRA-OutlookSendReceive) [Microsofti toe ja taastamise abimees](https://diagnostics.office.com/#/) tööriista mõjutatud arvutis.

Kui sõnum jääb teie väljundkaustas kinni, on kõige tõenäolisem põhjus suur manus või suvand "saada kohe, kui see on ühendatud" pole lubatud.

**Eemaldage suur manus**

1. Klõpsake nuppu **Saada/võta vastu** > **Tööta ühenduseta**. 
2. Klõpsake navigeerimispaanil nuppu **Outbox**. Siit saate: 
    - Kustutage sõnum. Lihtsalt valige see ja klõpsake nuppu **Kustuta**.
    - Lohistage sõnum oma **mustandite kausta**, topeltklõpsake sõnumi avamiseks ja kustutage manus (klõpsake seda ja klõpsake nuppu **Kustuta**).
3. Kui tõrge ütleb, et Outlook proovib sõnumit edastada, sulgege Outlook. Väljumiseks võib kuluda mõni hetk. Kui Outlook ei sulge, vajutage **klahvikombinatsiooni CTRL + ALT + DELETE** ja klõpsake nuppu **Käivita Tegumihaldur**. Tegumihaldur, valige vahekaart **protsessid** , kerige Outlook. exe ja klõpsake **Lõpeta protsess**.
4. Pärast Outlook sulgub, taaskäivitage Outlook ja korrake samme 2-3. 
5. Pärast manuse eemaldamist klõpsake nuppu **Saada/võta vastu** > **ühenduseta** , et tühistada nupp ja jätkata tööd veebis. 

Sõnumid jäävad ka väljundkasti, kui klõpsate nuppu **saada**, kuid te ei ole ühendatud. Klõpsake nuppu **Saada/võta vastu** ja vaadake **ühenduseta töö** nuppu. Kui see on sinine, siis sa oled lahutatud. Klõpsake seda ühendamiseks (nupp muutub valgeks) ja klõpsake **saada kõik**.
 
**Luba saatmine kohe, kui see on ühendatud**
 
1. Klõpsake menüü Fail käsku **Suvandid**.

2. Klõpsake dialoogiboksis Outlooki suvandid nuppu **Täpsemalt**.

3. Klõpsake jaotises saatmise ja vastuvõtu lubamiseks **Saada kohe, kui**see on ühendatud. Klõpsake nuppu **OK**.
 
Täielikud üksikasjad leiate teemast:
- [Video: saata või kustutada ummikus e-posti](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [E-posti jääb kausta saatmiseks kuni te käsitsi algatada saatmise/vastuvõtu toiming Outlookis](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
