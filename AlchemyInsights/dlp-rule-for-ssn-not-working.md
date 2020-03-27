---
title: DLP reegel SSN ei tööta
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
ms.openlocfilehash: 4ec0df9d4954a8c65f0c34188d285dd8cf44a4f2
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977302"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP probleemid sotsiaalkindlustuse numbrid

**Oluline**: nendel enneolematul ajal me võtame meetmeid, et tagada SharePoint Online ' i ja OneDrive teenused on väga kättesaadavad-Palun külastage [SharePoint Online ajutised funktsiooni kohandused](https://aka.ms/ODSPAdjustments) lisateabe saamiseks.

**DLP probleemid SSNs**

Kas teil on probleeme **andmete kadu vältimine (DLP)** ei tööta sisu, mis sisaldab **sotsiaalse turvalisuse number (SSN)** tundliku teabe tüüp Office 365 kasutamisel? Kui jah, veenduge, et teie sisu sisaldab vajalikku teavet DLP poliitika otsib. 
  
Näiteks SSN poliitika konfigureeritud usalduse tase 85%, hinnatakse ja tuleb tuvastada reegli käivitamiseks:
  
- **[Formaat:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 numbrit, mis võib olla vormindatud või vormindamata muster

- **[Muster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Neli funktsiooni otsima SSNs neljas erinevas struktuuris:

  - Func_ssn leiab SSNs pre-2011 tugeva vormingu, mis on vormindatud kriipsu või tühikuid (DDD-DD-dddd või DDD DD dddd)

  - Func_unformatted_ssn leiab SSNs pre-2011 tugev vormindamine, mis on vormindamata üheksa järjestikust numbrit (ddddddddd)

  - Func_randomized_formatted_ssn leiab post-2011 SSNs, mis on vormindatud kriipsude või tühikute (DDD-DD-dddd või DDD DD dddd)

  - Func_randomized_unformatted_ssn leiab post-2011 SSNs, mis on vormindamata üheksa järjestikust numbrit (ddddddddd)

- **[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Ei, kontrollsumma puudub

- **[Määratlus:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP poliitika on 85% kindel, et see on avastatud seda tüüpi tundlik teave, kui lähedus 300 tähemärki:

  - [Funktsioon Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) otsib sisu, mis vastab mustrile.

  - Leitakse märksõna [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) . Märksõnade näited on: *sotsiaalkindlustus, sotsiaalkindlustus #, SOC SEC, SSN* . Näiteks järgmine näidis käivitab DLP SSN poliitika: **SSN: 489-36-8350**
  
Lisateabe saamiseks selle kohta, mida on vaja SSNs tuvastatav sisu, lugege järgmist jaotist selles artiklis: [mida tundliku teabe tüübid otsida SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Kasutades muu sisseehitatud tundliku teabe tüüp, lugege järgmist artiklit teavet, mida on vaja muud tüüpi: [mida tundliku teabe tüübid otsida](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  