---
title: DLP reegel krediitkaardi number ei tööta
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 80ff41b3e746f95278ccbf0df19eebb61f7f9ee0
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704197"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP probleemid krediitkaardi numbrid

**Tähtis**! Nende enneolematude aegade jooksul võtame kasutusele meetmed, et säilitada SharePoint Online’i ja OneDrive’i teenuste hea kättesadavus. Lisateabe saamiseks vaadake teemat [SharePoint Online’i ajutised funktsioonide muudatused](https://aka.ms/ODSPAdjustments).

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
  