---
title: DLP reegel, et krediitkaardi number ei tööta
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
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679437"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Krediitkaardi numbritega seotud DLP

**Tähtis**! Nende enneolematude aegade jooksul võtame kasutusele meetmed, et säilitada SharePoint Online’i ja OneDrive’i teenuste hea kättesadavus. Lisateabe saamiseks vaadake teemat [SharePoint Online’i ajutised funktsioonide muudatused](https://aka.ms/ODSPAdjustments).

**Krediitkaardi numbritega seotud DLP**

Kas teil on probleeme **andmete kaotsimineku vältimisega (DLP)** , mis ei tööta **krediitkaardi numbrit** sisaldava sisuga, kui kasutate O365 DLP tundliku teabe tüüpi? Kui jah, siis veenduge, et teie sisu sisaldaks vajalikku teavet, et käivitada DLP poliitika, kui seda hinnatakse. Näiteks, kui teie **krediitkaardi poliitika** on konfigureeritud 85%, hinnatakse ja see tuleb reegli käivitamiseks tuvastada järgmiselt.
  
- **[Vorming:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 numbrit, mis võivad olla vormindatud või vormindamata (dddddddddddddddd) ja peavad läbima Luhn testi.

- **[Muster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Väga keerukas ja jõuline muster, mis tuvastab kogu maailmas kaarte, sh Visa, MasterCard, Discover Card, JCB, American Express, Kinkekaardid ja söökla kaardid.

- **[Kontrollsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Jah, Luhn kontrollsumma

- **[Definitsioon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** DLP poliitika on 85% kindel, et see on tuvastanud seda tüüpi tundliku teabe, kui 300 märkide lähedusse jääb:

  - Funktsioon Func_credit_card otsib mustriga kattuvat sisu.

  - Kehtib mõni järgmistest.

  - Leitakse Keyword_cc_verification märksõna.

  - Leitakse Keyword_cc_name märksõna

  - Funktsioon Func_expiration_date leiab kuupäeva õigel kuupäevavorming.

  - Kontrollsumma läbib

    Näiteks käivitatakse järgmise valimi korral DLP krediitkaardi numbri poliitika.

  - Visa: 4485 3647 3952 7352
  
  - Aegub: 2/2009

Lisateavet selle kohta, mida on vaja teie **teabesisu tuvastamiseks** , leiate selle artikli jaotisest [Kuidas tundlikud andmetüübid välja näevad?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Mõne muu sisseehitatud tundliku teabe tüübi abil leiate lisateavet selle kohta, mida on vaja muude tüüpide jaoks: [millist tüüpi tundlikud teabe tüübid otsivad](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  