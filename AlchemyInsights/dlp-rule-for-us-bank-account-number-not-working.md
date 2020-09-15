---
title: DLP reegel US Bank Account number ei tööta
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679292"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP probleemid US Banki konto numbritega

**Tähtis**! Nende enneolematude aegade jooksul võtame kasutusele meetmed, et säilitada SharePoint Online’i ja OneDrive’i teenuste hea kättesadavus. Lisateabe saamiseks vaadake teemat [SharePoint Online’i ajutised funktsioonide muudatused](https://aka.ms/ODSPAdjustments).

**DLP probleemid US Banki konto numbritega**

Kas teil on probleeme **andmete kaotsimineku vältimisega (DLP)** , mis ei tööta **USA** kontonumbrit sisaldava sisuga, kui kasutate O365 DLP tundliku teabe tüüpi? Kui jah, siis veenduge, et teie sisu sisaldaks vajalikku teavet selle kohta, mida DLP poliitika selle hindamisel otsib.
  
Näiteks kui **US Bank Account number** on konfigureeritud 85% usaldusväärsusega, hinnatakse ja tuleb reegli käivitamise korral tuvastada järgmist.
  
- **[Vorming:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 numbrit

- **[Muster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 järjestikused numbrid.

- **[Kontrollsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ei, pole kontrollsummat

- **[Definitsioon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** DLP poliitika on 75% kindel, et see on tuvastanud seda tüüpi tundliku teabe, kui 300 märkide lähedusse jääb:

  - Tavaline avaldis Regex_usa_bank_account_number otsib mustriga kattuvat sisu.

  - Leitakse Keyword_usa_Bank_Account märksõna.

    Näiteks käivitab Järgmine näidis **USA pangakonto numbripoliitika** : konto 78344011

Lisateavet selle kohta, mis on vajalik selle kohta, mis on vajalik teie sisu tuvastamiseks **USA pangakonto numbri** kohta, leiate selle artikli jaotisest [Kuidas tundlikud teabe liigid meie pangakonto numbrit näevad](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number) ?
  
Mõne muu sisseehitatud tundliku teabe tüübi abil leiate lisateavet selle kohta, mida on vaja muude tüüpide jaoks: [millist tüüpi tundlikud teabe tüübid otsivad](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  