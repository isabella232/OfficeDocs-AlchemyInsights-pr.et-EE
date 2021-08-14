---
title: SSN-i DLP-reegel ei tööta
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
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004978"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP-probleemid sotsiaalkindlustuse numbritega

**Tähtis**! Nende enneolematude aegade jooksul võtame kasutusele meetmed, et säilitada SharePoint Online’i ja OneDrive’i teenuste hea kättesadavus. Lisateabe saamiseks vaadake teemat [SharePoint Online’i ajutised funktsioonide muudatused](https://aka.ms/ODSPAdjustments).

**SSN-ide DLP-probleemid**

Kas teil on probleeme andmete kaotsimineku **vältimisega (DLP),** mis ei tööta **SSN-i (SSN)** sisaldava sisu korral, kui kasutate Microsoft 365? Sel juhul veenduge, et teie sisu sisaldaks vajalikku teavet selle kohta, mida DLP-poliitika otsib. 
  
Näiteks SSN-i poliitika puhul, mis on konfigureeritud usaldustasemega 85%, hinnatakse järgmist ja see tuleb tuvastada, et reegel käivituks.
  
- **[Vorming:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 numbrit, mis võivad olla vormindatud või vormindamata mustris

- **[Muster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Neli funktsiooni näevad SSN-id välja neljas erinevas mustrites.

  - Func_ssn 2011. aasta eelse tugeva vorminguga SSN-id, mis on vormindatud kriipsude või tühikutega (ddd-dd-ddddd OR ddd dd dddd)

  - Func_unformatted_ssn 2011. aasta eelse tugeva vorminguga SSN-id, mis on vormindamata üheksa järjestikuse numbrina (ddddddddd)

  - Func_randomized_formatted_ssn 2011. aasta järgsed SSN-id, mis on vormindatud kriipsude või tühikutega (ddd-dd-ddddd OR ddd dd dddd)

  - Func_randomized_unformatted_ssn leiab pärast 2011. aasta SSN-e, mis on vormindamata üheksa järjestikuse numbrina (ddddddddddd)

- **[Kontrollsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Ei, kontrollsummat pole

- **[Definitsioon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP-poliitika on 85% kindel, et tuvastatakse seda tüüpi tundlik teave, kui 300 märgi läheduses:

  - Funktsioon [Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) sisu, mis vastab mustrile.

  - Leitakse [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) märksõna. Märksõnade hulka kuuluvad näiteks:  *Sotsiaalkindlustus, Sotsiaalkindlustus#, Soc Sec , SSN*  . Näiteks järgmine näide käivitaks DLP SSN-i poliitika: **SSN: 489-36-8350**
  
Lisateavet selle kohta, mida on vaja SSN-ide tuvastamiseks sisu jaoks, leiate selle artikli järgmisest jaotisest: Tundliku teabe tüübid [SSN-ide otsimise kohta](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Muu tundliku loomuga teabetüübi kasutamise kohta leiate teavet selle kohta, mida muud tüüpi tundliku sisuga teabetüübid [on nõutavad.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  