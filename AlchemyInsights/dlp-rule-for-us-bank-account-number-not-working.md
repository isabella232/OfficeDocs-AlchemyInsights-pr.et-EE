---
title: DLP reegel USA pangakonto number ei tööta
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
ms.openlocfilehash: bb7d8ca91af73fa4ebed5992ec848128beb18830
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977158"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP probleemid USA pangakonto numbrid

**Oluline**: nendel enneolematul ajal me võtame meetmeid, et tagada SharePoint Online ' i ja OneDrive teenused on väga kättesaadavad-Palun külastage [SharePoint Online ajutised funktsiooni kohandused](https://aka.ms/ODSPAdjustments) lisateabe saamiseks.

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
  