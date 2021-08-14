---
title: DLP-reegel USA pangakonto numbrile ei tööta
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
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005014"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP-probleemid USA pangakontonumbritega

**Tähtis**! Nende enneolematude aegade jooksul võtame kasutusele meetmed, et säilitada SharePoint Online’i ja OneDrive’i teenuste hea kättesadavus. Lisateabe saamiseks vaadake teemat [SharePoint Online’i ajutised funktsioonide muudatused](https://aka.ms/ODSPAdjustments).

**DLP-probleemid USA pangakontonumbritega**

Kas teil on probleeme andmete kaotsimineku **vältimisega (DLP),** mis ei tööta O365-s DLP-tundliku teabe tüübi kasutamisel USA pangakontonumbrit sisaldava sisu korral?  Sel juhul veenduge, et teie sisu sisaldaks vajalikku teavet selle kohta, mida DLP-poliitika selle hindamise ajal otsib.
  
Näiteks usa pangakontonumbri poliitika puhul, mis on konfigureeritud usaldustasemega 85%, hinnatakse järgmist ja see tuleb tuvastada, et reegel käivituks. 
  
- **[Vorming:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8–17 numbrit

- **[Muster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8–17 järjestikust numbrit.

- **[Kontrollsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ei, kontrollsummat pole

- **[Definitsioon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** DLP-poliitika on 75% kindel, et tuvastatakse seda tüüpi tundlik teave, kui 300 märgi läheduses:

  - Regulaaravaldise abil Regex_usa_bank_account_number sisu, mis vastab mustrile

  - Leitakse Keyword_usa_Bank_Account märksõna.

    Näiteks käivitaks USA pangakontonumbri poliitika **järgmine** näide: Kontonumbrite 78344011

Lisateavet selle kohta, mida  on vaja teie sisu tuvastamiseks USA pangakontonumbri tuvastamiseks, leiate selle artikli järgmisest jaotisest: Mis on tundliku sisuga teabetüübid [usa pangakonto numbri jaoks?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Muu tundliku loomuga teabetüübi kasutamise kohta leiate teavet selle kohta, mida muud tüüpi tundliku sisuga teabetüübid [on nõutavad.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  