---
title: e-juurdluse ekspordi tööriist
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: f7b7e1ae4f1f686fa510403d398c4ff750dbadb9065b8d63701a927eeac52d9b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101298"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Kas te ei saa e-juurdluse ekspordi tööriista installida või käivitada?

Kui te ei saa otsingutulemite allalaadimiseks e-juurdluse ekspordi tööriista installida ega käivitada, kontrollige järgmist.
  
- Arvuti, mida kasutate, vastab rekvisiitide nõuetele.

  - 32- või 64-bitised versioonid Windows 7 ja uuemates versioonides

  - Microsoft .NET Framework 4.7

  - Toetatud brauser:

  - Microsoft Edge

    Või

  - Internet Explorer 10 ja uuemad versioonid

    Muid brausereid (nt Google Chrome ja Mozilla Firefox) ei toetata.

- Teie ettevõte saab luua ühenduse Azure'i lõpp-punktiga, **\* mis on .blob.core.windows.net** (metamärk tähistab teie eksporditöö kordumatut identifikaatorit).

- Teile määratakse ekspordiroll Microsoft 365 &amp; turbenõuete keskuses. Vaikimisi määratakse see roll ainult e-juurdluse halduri rollirühmale. Lugege [teemat E-juurdluse õiguste määramine.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)

Lisateavet leiate teemast [Sisuotsingu tulemite eksportimine.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)

Kui ekspordite rohkem kui 100 K postkasti, peate tulemite eksportimiseks kasutama järgmist PowerShelli: tulemite eksportimine rohkem kui [100K postkastidest.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)