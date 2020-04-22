---
title: DLP reegel USA pangakonto number ei tööta
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 45aa50f6c3505468e902e58faf698205f93f9264
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704035"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP probleemid USA pangakonto numbrid

**Tähtis**! Nende enneolematude aegade jooksul võtame kasutusele meetmed, et säilitada SharePoint Online’i ja OneDrive’i teenuste hea kättesadavus. Lisateabe saamiseks vaadake teemat [SharePoint Online’i ajutised funktsioonide muudatused](https://aka.ms/ODSPAdjustments).

**DLP probleemid USA pangakonto numbrid**

Kas teil on probleeme **andmete kadu vältimine (DLP)** ei tööta sisu, mis sisaldab **USA pangakonto number** , kui kasutate DLP tundliku teabe tüüp O365? Kui jah, veenduge, et teie sisu sisaldab vajalikku teavet selle kohta, mida DLP poliitika otsib, kui seda hinnatakse.
  
Näiteks **USA pangakonto number** poliitika konfigureeritud usalduse tase 85%, hinnatakse järgmist ja tuleb tuvastada reegli käivitamiseks:
  
- **[Formaat:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 numbrit

- **[Muster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 järjestikust numbrit.

- **[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ei, kontrollsumma puudub

- **[Määratlus:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP poliitika on 75% kindel, et see on avastatud seda tüüpi tundlik teave, kui lähedus 300 tähemärki:

  - Regulaarne avaldis Regex_usa_bank_account_number otsib sisu, mis vastab muster

  - Leitakse märksõna Keyword_usa_Bank_Account.

    Näiteks järgmine näidis käivitab **USA pangakonto number** poliitika: konto 78344011 kontrollimine

Lisateabe saamiseks selle kohta, mida on vaja **USA pangakonto number** tuvastatav teie sisu, lugege järgmist jaotist selles artiklis: [mida tundliku teabe tüübid otsida USA pangakonto number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Kasutades muu sisseehitatud tundliku teabe tüüp, lugege järgmist artiklit teavet, mida on vaja muud tüüpi: [mida tundliku teabe tüübid otsida](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  