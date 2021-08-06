---
title: Töövoog ei käivitu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 77a3c022a9a3a82041b4a4a70c72c2e0940c0fba27f296f07881e3abebf1e464
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53907734"
---
# <a name="workflow-is-not-starting"></a>Töövoog ei käivitu

- SharePoint 2010 ja SharePoint 2013 töövood ei käivitu.

    - Kui töövoog ei käivitu, võib ilmneda ajutine teenuseprobleem, mille korral kasutajad võivad töövoo edenemise korral ilmneda aeg-ajalt viivitusi. Kontrollige [teenuse seisundi armatuurlauda,](https://admin.microsoft.com/AdminPortal/Home/servicehealth) et näha, kas teie ettevõtet mõjutab.

    - Kui sellest probleemist on möödunud rohkem kui 24 tundi, logige sisse tugiteenusepilet. Paljudel juhtudel töötame juba lahenduse kallal. Lahenduse lõpuleviimiseks andke meile vähemalt 24 tundi.

- SharePoint 2010 töövood viivitusega käivitamisel.

    - See juhtub siis, kui töövoog käivitatakse suurtes pakettides. (nt kui korraga lisatakse mitu üksust).

    - Töövood pole loodud reaalajas töötama, nii et viivitus on by-design käitumine.

   -  Kui töövoog on keerukas laiendatav objekti märgistuskeel (XMOL), võib kompileerimine olla aeglane. Vaadake [seda](https://support.microsoft.com//kb/3043697) artiklit.

    - Peaksite töövoogu lihtsustama või selle ümber kujundama Microsoft SharePoint 2013 töövooplatvormi tüübi abil.

    - Kui töövoo ajalugu on kasvanud suureks, võite soovida üksused likvideerida või luua uue ajalooloendi.

        Lisateave: [Töövooajaloo likvideerimine](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Seotud teemad
Kas soovite proovida Microsoft Flow SharePoint Online'is?
- [Loo Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ja Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
