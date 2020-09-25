---
title: e-juurdluse ekspordi tööriist
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277946"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>E-juurdluse ekspordi tööriista ei saa installida või käivitada?

Kui te ei saa otsingutulemite allalaadimiseks e-juurdluse ekspordi tööriista installida ega käivitada, kontrollige järgmisi asju.
  
- Arvuti, mida kasutate, vastab järgmistele eeltingimustele:

  - 32-või 64-bitised versioonid Windows 7 ja uuemad versioonid

  - Microsoft .NET Framework 4.7

  - Toetatud brauser.

  - Microsoft Edge

    Või

  - Internet Explorer 10 ja uuemad versioonid

    Muud brauserid (nt Google Chrome ja Mozilla Firefox) ei toeta.

- Teie asutus saab luua ühenduse lõpp-punktiga Azure ' is, mis on ** \* . blob.Core.Windows.net** (metamärki tähistab teie eksporditoimingu kordumatut identifikaatorit).

- Olete määranud ekspordi rolli Microsoft 365 turbe &amp; nõuetele vastavuse keskuses. Vaikimisi määratakse see roll ainult e-juurdluse halduri rollirühma. Vaadake teemat e- [juurdluse õiguse määramine](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Lisateavet leiate teemast [sisu otsingutulemite eksportimine](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).

Kui ekspordite rohkem kui 100K postkaste, peate eksportimise tulemite allalaadimiseks kasutama järgmist PowerShelli, et eksportida  [tulemid enam kui 100k postkastist](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).