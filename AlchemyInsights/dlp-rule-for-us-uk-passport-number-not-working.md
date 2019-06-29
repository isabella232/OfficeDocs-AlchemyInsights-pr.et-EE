---
title: DLP reegel USA / UK passi Number ei tööta
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 0567e9521507bcc192b187d0e5a8a0658332ff99
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389537"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>DLP - probleemid U.S. / UK passi numbrid

On teil probleeme **Andmete kaotsimineku vältimise (DLP)** ei tööta sisu sisaldava puhul on **U.S. / UK passi Number** kasutades DLP tundliku teabe tüüp O365? Sellisel juhul veenduge, et sisu sisaldab vajalikku teavet kui hinnatakse seda, mida otsib DLP poliitika.
  
Näiteks on **U.S. / UK passi Number** konfigureeritud 75% usaldusnivoo, järgmine hinnatakse ja reegli käivitamiseks tuleb kindlaks
  
- **[Formaat:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Üheksa numbrit

- **[Puhul:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Üheksa järjestikust numbrit

- **[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ei, ei ole kontrollsumma

- **[Määratlus:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP poliitika on 75% kindel, et ta ei avastanud seda tüüpi tundlikku teavet kui raadiuses 300 tähemärki:

  - Funktsiooni Func_usa_uk_passport leiab sisu, mis ühtiks.

  - Märksõna: Keyword_passport ei leitud.

    Näiteks peale tingiksid jaoks on **U.S. / UK passinumber** poliitika: USA passi number 123456789

Rohkem infot mis tuleb USA / UK passi Number tuvastada sisu, vt käesoleva artikli järgmist osa: [mida the tundliku teabe tüübid vaadata USA / UK passi Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Kasutades erinevaid sisseehitatud tundliku teabe tüüp, lugege järgmist teabe kohta, mida nõutakse muude: [mida the tundlik tüüpi teavet otsida](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  