---
title: DLP reegel numbrid ei tööta
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
ms.openlocfilehash: 875afb47175a78c22894720cb0db8222f6f41614
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529951"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP probleeme numbrite

On teil probleeme **Andmete kaotsimineku vältimise (DLP)** , mis sisaldab **Krediitkaardi numbrit** kasutades DLP tundliku teabe tüüp O365 sisu ei tööta? Sellisel juhul veenduge, et sisu sisaldab käivitamiseks vajalik teave ning kui seda hinnatakse DLP poliitika. Näiteks **krediitkaardi poliitika** konfigureeritud 85% usaldusnivoo, järgnev hinnatakse ja peavad avastama reegli käivitamiseks:
  
- **[Formaat:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16-kohaline, mida saab vormindada või vormindamata (dddddddddddddddd) ja peab läbima Luhn testi.

- **[Puhul:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Väga keeruline ja tugev muster, mis tuvastab kõik suure brändi üle maailma, sealhulgas Visa, MasterCard, Discover Card, JCB, American Express, Kinkekaardid ja söökla kaardid kaardid.

- **[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Jah, Luhn kontrollsumma

- **[Määratlus:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP poliitika on 85% kindel, et ta ei avastanud seda tüüpi tundlikku teavet kui raadiuses 300 tähemärki:

  - Funktsiooni Func_credit_card leiab sisu, mis ühtiks.

  - Üks järgmistest on tõsi:

  - Märksõna: Keyword_cc_verification ei leitud.

  - Märksõna: Keyword_cc_name on leitud

  - Funktsiooni Func_expiration_date leiab õige kuupäev vormingus kuupäev.

  - Kontrollsumma läheb

    Näiteks peale tingiksid DLP krediitkaardi Number poliitika:

  - Viisa: 4485 3647 3952 7352
  
  - Aegub: 2/2009

Mis tuleb **Numbrid** tuvastada sisu kohta lisateabe saamiseks vt käesoleva artikli järgmist osa: [Mida the tundliku teabe tüübid otsima krediitkaardi #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Kasutades erinevaid sisseehitatud tundliku teabe tüüp, lugege järgmist teabe kohta, mida nõutakse muude: [mida the tundlik tüüpi teavet otsida](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  