---
title: DLP reegel meid pangakonto Number ei tööta
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 83050b05cffacd3e81d34f05383c213eb0042fae
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389465"
---
On teil probleeme **Andmete kaotsimineku vältimise (DLP)** mis sisaldab **USA pangakonto numbrit** kasutades DLP tundliku teabe tüüp O365 sisu ei tööta? Sellisel juhul veenduge, et sisu sisaldab vajalikku teavet kui hinnatakse seda, mida otsib DLP poliitika.
  
Näiteks **USA pangakonto Number** poliitika konfigureeritud 85% usaldusnivoo, järgnev hinnatakse ja peavad avastama reegli käivitamiseks:
  
- **[Formaat:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 numbrit

- **[Muster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 järjestikust numbrit.

- **[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ei, ei ole kontrollsumma

- **[Määratlus:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP poliitika on 75% kindel, et ta ei avastanud seda tüüpi tundlikku teavet kui raadiuses 300 tähemärki:

  - Regulaaravaldise Regex_usa_bank_account_number leiab sisu, mis ühtiks

  - Märksõna: Keyword_usa_Bank_Account ei leitud.

    Näiteks peale tingiksid **USA pangakonto Number** poliitika: pangakonto 78344011

Lisateavet selle kohta, mida nõutakse **USA pangakonto Number** sisu tuvastada, leiate käesoleva artikli järgnevalt: [Mida the tundlik tüüpi teavet otsida USA pangakonto Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Kasutades erinevaid sisseehitatud tundliku teabe tüüp, lugege järgmist teabe kohta, mida nõutakse muude: [mida the tundlik tüüpi teavet otsida](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  