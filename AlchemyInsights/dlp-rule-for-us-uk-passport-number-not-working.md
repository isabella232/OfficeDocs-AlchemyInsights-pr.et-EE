---
title: DLP-reegel USA/UK passinumbri jaoks ei tööta
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
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004942"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Probleemid DLP-ga – USA/UK passinumbrid

**Tähtis**! Nende enneolematude aegade jooksul võtame kasutusele meetmed, et säilitada SharePoint Online’i ja OneDrive’i teenuste hea kättesadavus. Lisateabe saamiseks vaadake teemat [SharePoint Online’i ajutised funktsioonide muudatused](https://aka.ms/ODSPAdjustments).

**DLP-probleemid USA/Ühendkuningriigi passinumbritega**

Kas teil on probleeme andmete kaotsimineku **vältimisega (DLP),** mis ei tööta O365-s DLP-tundliku teabe tüübi kasutamisel **USA/Ühendkuningriigi** passinumbrit sisaldava sisu korral? Sel juhul veenduge, et teie sisu sisaldaks vajalikku teavet selle kohta, mida DLP-poliitika selle hindamise ajal otsib.
  
Näiteks **usa/Ühendkuningriigi** passinumbripoliitika puhul, mis on konfigureeritud usaldustasemega 75%, hinnatakse järgmist ja see tuleb tuvastada, et reegel käivitaks
  
- **[Vorming:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Üheksa numbrit

- **[Muster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Üheksa järjestikust numbrit

- **[Kontrollsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ei, kontrollsummat pole

- **[Definitsioon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** DLP-poliitika on 75% kindel, et tuvastatakse seda tüüpi tundlik teave, kui 300 märgi läheduses:

  - Funktsioon Func_usa_uk_passport sisu, mis vastab mustrile.

  - Leitakse Keyword_passport märksõna.

    Näiteks käivitaks USA/Ühendkuningriigi  passinumbripoliitika järgmine näidis: USA passide number 123456789

Lisateavet selle kohta, mida on vaja teie sisu tuvastamiseks USA/Ühendkuningriigi passinumbri tuvastamiseks, leiate selle artikli järgmisest jaotisest: Mis on tundliku sisuga teabetüübid [USA/Ühendkuningriigi passinumbri jaoks?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Muu tundliku loomuga teabetüübi kasutamise kohta leiate teavet selle kohta, mida muud tüüpi tundliku sisuga teabetüübid [on nõutavad.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  