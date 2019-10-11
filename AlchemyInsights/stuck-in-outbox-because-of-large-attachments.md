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
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441302"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Sõnumite parandamine, mis on väljundkaustas kinni

Soovitame alustada, käivitades stsenaariumi ["Mul on probleeme saatmine, vastuvõtmine või leidmine"](https://aka.ms/SaRA-OutlookSendReceive) [Microsofti toe ja taastamise abimees](https://diagnostics.office.com/#/) tööriista.

Kui sõnum jääb teie väljundkaustas kinni, on kõige tõenäolisem põhjus:
- Suured manused.
- **Saada kohe, kui ühendatud** suvand pole lubatud.

Suurte manuste eemaldamiseks toimige järgmiselt. 

1. Outlookis valige **saatmise/vastuvõtu** > **töö ühenduseta**. 
2. Valige navigeerimispaanil suvand **Väljundboks**. Siit saate: 
    - Kustutage sõnum (valige see ja seejärel valige **Kustuta**).
    - Lohistage sõnum mustandite kausta, topeltklõpsake selle avamiseks ja manuse eemaldamiseks valige see ja seejärel valige **Kustuta**).
3. Kui kuvatakse tõrketeade, mis ütleb, et Outlook proovib sõnumit edastada, sulgege Outlook. Väljumiseks võib kuluda mõni hetk. Kui Outlook ei sulge, vajutage klahvikombinatsiooni CTRL + ALT + DELETE ja valige **Käivita Tegumihaldur**. Valige Tegumihalduris vahekaart **protsessid** , kerige allapoole Outlook. exe ja valige **Lõpeta protsess**.
4. Pärast Outlooki sulgemist taaskäivitage see ja korrake juhiseid 2 ja 3. 
5. Pärast manuse eemaldamist klõpsake nuppu **Saada/võta vastu** > **Tööta ühenduseta** , et jätkata töötamist ühendusega. 

Sõnumid jäävad ka väljundkasti, kui klõpsate nuppu **saada**, kuid te ei ole ühendatud. Klõpsake nuppu **Saada/võta vastu** ja vaadake **ühenduseta töö** nuppu. Kui see on sinine, siis sa oled lahutatud. Valige see ühendamiseks (nupp muutub valgeks) ja klõpsake nuppu **saada kõik**.
 
Et lubada **saatmise kohe, kui**see on ühendatud:
 
- Valige >  **Täpsemad** **Failisuvandid** > ****.
Jaotises **saatmise ja vastuvõtu** valige **Saada kohe, kui**see on ühendatud, ja seejärel valige **OK**.
 
Täielikud üksikasjad on järgmised:
- [Video: saata või kustutada ummikus e-posti](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [E-posti jääb kausta saatmiseks kuni te käsitsi algatada saatmise/vastuvõtu toiming Outlookis](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
