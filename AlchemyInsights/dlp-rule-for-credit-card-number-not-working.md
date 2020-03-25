---
title: DLP reegel krediitkaardi number ei tööta
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932439"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP probleemid krediitkaardi numbrid

**Oluline**: paljud SharePoint Online ' i ja OneDrive kliendid käivitada Business kriitilised rakendused teenuse, mis töötavad taustal. Nende hulka kuuluvad sisu migratsioon, andmete kadu vältimine (DLP) ja backup lahendused. Nendel enneolematul ajal me võtame meetmeid, et tagada SharePoint Online ' i ja OneDrive teenused on väga kättesaadav ja usaldusväärne oma kasutajatele, kes sõltuvad teenuse rohkem kui kunagi varem kaugtöö stsenaariume.

Selle eesmärgi toetuseks oleme rakendanud ranget ahendamise piiranguid taustal olevatele rakendustele (migratsioon, DLP ja backup lahendused) tööpäeval päeva jooksul. Te peaksite ootama, et need rakendused saavutavad nende aegade jooksul väga piiratud läbilaskevõime. Aga, õhtuti ja nädalavahetusel tundi piirkonna, teenus on valmis töötlema oluliselt suurem hulk taotlusi taustal apps.

**DLP probleemid krediitkaardi numbrid**

Kas teil on probleeme **andmete kadu vältimine (DLP)** ei tööta sisu, mis sisaldab **krediitkaardi number** , kasutades DLP tundliku teabe tüüp O365? Kui jah, veenduge, et teie sisu sisaldab vajalikku teavet, et käivitada DLP poliitika, kui see on hinnatud. Näiteks **krediitkaardi poliitika** konfigureeritud usalduse tase 85%, hinnatakse ja tuleb tuvastada reegli käivitamiseks:
  
- **[Formaat:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 numbrit, mida saab vormindada või vormindamata (dddddddddddddddd) ja peab läbima Luhn test.

- **[Muster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Väga keeruline ja jõuline muster, mis tuvastab kaarte kõigi suuremate kaubamärkide kogu maailmas, sealhulgas Visa, MasterCard, Discover kaart, JCB, American Express, kinkekaardid, ja söökla kaardid.

- **[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Jah, Luhn-i kontrollsumma

- **[Määratlus:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP poliitika on 85% kindel, et see on avastatud seda tüüpi tundlik teave, kui lähedus 300 tähemärki:

  - Funktsioon Func_credit_card otsib sisu, mis vastab mustrile.

  - Üks järgmistest on täidetud:

  - Leitakse märksõna Keyword_cc_verification.

  - Leitakse märksõna Keyword_cc_name

  - Funktsioon Func_expiration_date otsib kuupäeva paremas kuupäevavormingus.

  - Kontrollsumma möödub

    Näiteks järgmine näidis käivitab DLP krediitkaardi number poliitika:

  - Viisa: 4485 3647 3952 7352
  
  - Aegub: 2/2009

Lisateabe saamiseks selle kohta, mida on vaja teie sisu tuvastada **krediitkaardi number** , lugege järgmist jaotist selles artiklis: [mida tundliku teabe tüübid otsida krediitkaardi #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Kasutades muu sisseehitatud tundliku teabe tüüp, lugege järgmist artiklit teavet, mida on vaja muud tüüpi: [mida tundliku teabe tüübid otsida](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  