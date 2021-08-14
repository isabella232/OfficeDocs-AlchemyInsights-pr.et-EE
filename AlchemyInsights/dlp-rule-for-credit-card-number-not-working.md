---
title: Krediitkaardinumbri DLP-reegel ei tööta
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005086"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP-probleemid krediitkaardinumbritega

**Tähtis**! Nende enneolematude aegade jooksul võtame kasutusele meetmed, et säilitada SharePoint Online’i ja OneDrive’i teenuste hea kättesadavus. Lisateabe saamiseks vaadake teemat [SharePoint Online’i ajutised funktsioonide muudatused](https://aka.ms/ODSPAdjustments).

**DLP-probleemid krediitkaardinumbritega**

Kas teil on probleeme andmete kaotsimineku **vältimisega (DLP),** mis ei tööta O365-s DLP-tundliku teabe tüübi kasutamisel krediitkaardinumbrit sisaldava sisu korral?  Sel juhul veenduge, et teie sisu sisaldab DLP-poliitika käivitamiseks vajalikku teavet, kui seda hinnatakse. Näiteks kui **krediitkaardipoliitika** on konfigureeritud usaldustasemega 85%, hinnatakse järgmist ja see tuleb tuvastada, et reegel käivituks.
  
- **[Vorming:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 numbrit, mida saab vormindada või vormindamata (dddddddd) ja peab läbima Luhni testi.

- **[Muster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Väga keerukas ja töökindel muster, mis tuvastab kaardid kõigilt suurematelt kaubamärkidelt üle kogu maailma, sh Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.

- **[Kontrollsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Jah, Luhni kontrollsumma

- **[Definitsioon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** DLP-poliitika on 85% kindel, et tuvastatakse seda tüüpi tundlik teave, kui 300 märgi läheduses:

  - Funktsioon Func_credit_card sisu, mis vastab mustrile.

  - Üks järgmistest on tõene.

  - Leitakse Keyword_cc_verification märksõna.

  - Otsitakse Keyword_cc_name märksõna

  - Funktsioon Func_expiration_date kuupäeva õiges kuupäevavormingus.

  - Kontrollsumma läbib

    Näiteks käivitaks järgmine näide DLP krediitkaardinumbri poliitika.

  - Visa: 4485 3647 3952 7352
  
  - Aegub: 2.02.2009

Lisateavet selle kohta, mida on vaja, et teie sisu jaoks tuvastataks **krediitkaardinumber,** leiate selle artikli järgmisest jaotisest: Mida tundliku teabe tüübid krediitkaardi [jaoks näevad?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Muu tundliku loomuga teabetüübi kasutamise kohta leiate teavet selle kohta, mida muud tüüpi tundliku sisuga teabetüübid [on nõutavad.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  