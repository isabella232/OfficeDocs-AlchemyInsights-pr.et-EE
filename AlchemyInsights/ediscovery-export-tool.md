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
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814584"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Kas te ei saa e-juurdluse ekspordi tööriista installida või käivitada?

Kui te ei saa otsingutulemite allalaadimiseks e-juurdluse ekspordi tööriista installida ega käivitada, kontrollige järgmist.
  
- Arvuti, mida kasutate, vastab rekvisiitide nõuetele.

  - Windows 7 ja uuemate versioonide 32- või 64-bitised versioonid

  - Microsoft .NET Framework 4.7

  - Toetatud brauser:

  - Microsoft Edge

    Või

  - Internet Explorer 10 ja uuemad versioonid

    Muid brausereid (nt Google Chrome ja Mozilla Firefox) ei toetata.

- Teie ettevõte saab luua ühenduse Azure'i lõpp-punktiga, **\* mis on .blob.core.windows.net** (metamärk tähistab teie eksporditöö kordumatut identifikaatorit).

- Teile määratakse Microsoft 365 turbenõuete keskuses &amp; ekspordiroll. Vaikimisi määratakse see roll ainult e-juurdluse halduri rollirühmale. Lugege [teemat E-juurdluse õiguste määramine.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)

Lisateavet leiate teemast [Sisuotsingu tulemite eksportimine.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)

Kui ekspordite rohkem kui 100 K postkasti, peate tulemite eksportimiseks kasutama järgmist PowerShelli: tulemite eksportimine rohkem kui [100K postkastidest.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)