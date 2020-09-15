---
title: DLP reegel SSN ei tööta
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679365"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP seotud probleemid

**Tähtis**! Nende enneolematude aegade jooksul võtame kasutusele meetmed, et säilitada SharePoint Online’i ja OneDrive’i teenuste hea kättesadavus. Lisateabe saamiseks vaadake teemat [SharePoint Online’i ajutised funktsioonide muudatused](https://aka.ms/ODSPAdjustments).

**Vorminguga SSN DLP probleemid**

Kas teil on probleeme **andmete kaotsimineku vältimisega (DLP)** , mis ei tööta Microsoft 365 tundliku teabe tippimise korral **sotsiaalkindlustuse numbrit (SSN)** sisaldava sisuga? Kui jah, siis veenduge, et teie sisu sisaldaks vajalikku teavet selle kohta, mida DLP poliitika otsib. 
  
Näiteks SSN poliitika jaoks, mis on konfigureeritud 85%-ga, hinnatakse ja see tuleb reegli käivitamiseks tuvastada järgmiselt.
  
- **[Vorming:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 numbrit, mis võivad olla vormindatud või vormindamata mustriga.

- **[Muster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Neli funktsiooni otsivad vorminguga SSN neljast erinevast etalonist.

  - Func_ssn leiab vorminguga SSN, 2011 kus on DDD, kus on vormindatud kriipsud või tühikud (-DD-dddd või DDD DD dddd).

  - Func_unformatted_ssn leiab vorminguga SSN 2011, kus on ddddddddd tugev vorming, mis on vormindamata üheksa järjestikust numbrit ().

  - Func_randomized_formatted_ssn leiab post-2011 vorminguga SSN, mis on vormindatud sidekriipsude või tühikutega (DDD-DD-dddd või DDD DD dddd)

  - Func_randomized_unformatted_ssn leiab post-2011 vorminguga SSN, mis on vormindamata üheksa järjestikuseks numbriks (ddddddddd)

- **[Kontrollsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Ei, pole kontrollsummat

- **[Definitsioon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP poliitika on 85% kindel, et see on tuvastanud seda tüüpi tundliku teabe, kui 300 märkide lähedusse jääb:

  - [Funktsioon Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) otsib mustriga kattuvat sisu.

  - Leitakse [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) märksõna. Märksõnade näited on:  *sotsiaalkindlustus, sotsiaalkindlustus #, SOC SEC, SSN*  . Näiteks käivitatakse DLP SSN poliitika jaoks järgmine näidis: **SSN: 489-36-8350**
  
Lisateavet selle kohta, mida on vaja sisu tuvastamiseks vorminguga SSN, leiate selle artikli jaotisest [Kuidas tundlikud andmetüübid vorminguga SSN otsivad?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Mõne muu sisseehitatud tundliku teabe tüübi abil leiate lisateavet selle kohta, mida on vaja muude tüüpide jaoks: [millist tüüpi tundlikud teabe tüübid otsivad](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  