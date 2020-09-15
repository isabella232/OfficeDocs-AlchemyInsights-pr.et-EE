---
title: DLP reegel US/UK passi number ei tööta
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679220"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Probleemid DLP-US/UK Passporti numbritega

**Tähtis**! Nende enneolematude aegade jooksul võtame kasutusele meetmed, et säilitada SharePoint Online’i ja OneDrive’i teenuste hea kättesadavus. Lisateabe saamiseks vaadake teemat [SharePoint Online’i ajutised funktsioonide muudatused](https://aka.ms/ODSPAdjustments).

**DLP probleemid US/UK Passporti numbritega**

Kas teil on probleeme **andmete kaotsimineku vältimisega (DLP)** , mis ei tööta, kui teil on DLP tundliku teabe tüüpi O365 kasutamisel **US/UK Passporti numbrit** sisaldav sisu? Kui jah, siis veenduge, et teie sisu sisaldaks vajalikku teavet selle kohta, mida DLP poliitika selle hindamisel otsib.
  
Näiteks kui **US/UK Passporti kood** , mis on konfigureeritud 75% usalduse tasemega, hinnatakse ja seda tuleb reegli käivitamiseks tuvastada
  
- **[Vorming:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Üheksa numbrit

- **[Muster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Üheksa järjestikust numbrit

- **[Kontrollsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ei, pole kontrollsummat

- **[Definitsioon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** DLP poliitika on 75% kindel, et see on tuvastanud seda tüüpi tundliku teabe, kui 300 märkide lähedusse jääb:

  - Funktsioon Func_usa_uk_passport otsib mustriga kattuvat sisu.

  - Leitakse Keyword_passport märksõna.

    Näiteks käivitab järgmine valim **USA/Ühendkuningriigi passi numbripoliitika** : USA passi number 123456789

Lisateavet selle kohta, mida on vaja teie sisu tuvastamiseks US/UK Passporti numbri kohta, leiate selle artikli jaotisest [mis on tundlikud ANDMETÜÜBID meie/Ühendkuningriigi passi numbri](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number) järgi.
  
Mõne muu sisseehitatud tundliku teabe tüübi abil leiate lisateavet selle kohta, mida on vaja muude tüüpide jaoks: [millist tüüpi tundlikud teabe tüübid otsivad](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  