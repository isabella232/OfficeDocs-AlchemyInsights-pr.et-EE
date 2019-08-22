---
title: DLP reegel ei tööta SSN
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 757136c39700f12f40f839b29277a59b0e436f03
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529846"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP küsimusi isikukoodidega

On sul probleeme ei tööta sisu sisaldava **Isikukood (SSN)** , kasutades teatud tundlikku teavet Office 365 **Andmete kaotsimineku vältimise (DLP)** ? Sellisel juhul veenduge, et sisu sisaldab vajalikku teavet DLP poliitika turist. 
  
Nt SSN poliitikat konfigureeritud 85% usaldusnivoo, järgnev hinnatakse ja peavad avastama reegli käivitamiseks:
  
- **[Formaat:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 numbrit, mis võib olla vormindatud või vormindamata muster

- **[Puhul:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Neli funktsiooni otsima SSNs neli erinevat tasandit:

  - Func_ssn leiab SSNs eel-2011 tugev disain kriipse ega tühikuid (ddd-dd-dddd OR ddd dd dddd) vormindatud

  - Func_unformatted_ssn leiab SSNs eel-2011 tugev disain on vormindamata, nagu üheksa järjestikust numbrit (ddddddddd)

  - Func_randomized_formatted_ssn leiab post-2011 SSNs, mis on vormindatud kriipse ega tühikuid (ddd-dd-dddd OR ddd dd dddd)

  - Func_randomized_unformatted_ssn leiab post-2011 SSNs, mis on vormindamata, nagu üheksa järjestikust numbrit (ddddddddd)

- **[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Ei, ei ole kontrollsumma

- **[Määratlus:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP poliitika on 85% kindel, et ta ei avastanud seda tüüpi tundlikku teavet kui raadiuses 300 tähemärki:

  - [Funktsiooni Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) leiab sisu, mis ühtiks.

  - Märksõna: [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) ei leitud. Sisaldab näiteks märksõnu: *sotsiaalse turvalisuse, sotsiaalkindlustuse #, Soc Sec, SSN* . Näiteks peale tingiksid DLP SSN poliitika: **SSN: 489-36-8350**
  
Lisateavet selle kohta, mis tuleb SSNs sisu tuvastada, leiate järgnevalt selles artiklis: [Mida the tundlik tüüpi teavet otsida SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Kasutades erinevaid sisseehitatud tundliku teabe tüüp, lugege järgmist teabe kohta, mida nõutakse muude: [mida the tundlik tüüpi teavet otsida](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  