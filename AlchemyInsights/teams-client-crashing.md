---
title: Kas Teamsi klient jookseb kokku?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030587"
---
# <a name="teams-client-crashing"></a>Kas Teamsi klient jookseb kokku?

Kui teie Teamsi klient jookseb kokku, proovige järgmist.

- Kui kasutate Teamsi töölauarakendust, [veenduge, et rakendus oleks täielikult värskendatud](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Veenduge, et kõik [Office 365 URL-id ja aadresside vahemikud](https://docs.microsoft.com/microsoftteams/connectivity-issues) oleksid juurdepääsetavad.

- Logige oma administraatori kontoga sisse ja kontrollige oma [teenuse seisundi andmelauda](https://docs.microsoft.com/office365/enterprise/view-service-health), et teha kindlaks, kas ei esine katkestust ega teenuse jõudluse vähenemist.

 - Viimase toiminguna võite proovida tühjendada Teamsi kliendi vahemälu.

    1.  Väljuge täielikult Microsoft Teamsi töölauakliendist. Saate paremklõpsata ikoonide alal **Teamsi** ja klõpsata suvandit **Sulge** või käivitada tegumihalduri ja protsessi täielikult sulgeda.

    2.  Minge File Explorerisse ja sisestage %appdata%\Microsoft\teams.

    3.  Kataloogis kuvatakse üks järgmistest kaustadest.

         - Asukohas **Application Cache** (Rakenduse vahemälu) avage suvand Vahemälu ja kustutage kõik failid vahemälu asukohas: %appdata%\Microsoft\teams\application cache\cache.

        - Kustutage asukohas **Blob_storage** (Bloobimälu) kõik failid: %appdata%\Microsoft\teams\blob_storage.

        - Kustutage asukohas **Cache** (Vahemälu) kõik failid: %appdata%\Microsoft\teams\Cache.

        - Kustutage asukohas **databases** (Andmebaasid) kõik failid: %appdata%\Microsoft\teams\databases.

        - Kustutage asukohas **GPUCache** (GPU vahemälu) kõik failid: %appdata%\Microsoft\teams\GPUcache.

        - Kustutage asukohas **IndexedDB** (Indekseeritud DB) DB-fail: %appdata%\Microsoft\teams\IndexedDB.

        - Kustutage asukohas **Local Storage** (Kohalik mälu) kõik failid: %appdata%\Microsoft\teams\Local Storage.

        - Viimasena kustutage asukohas **tmp** kõik failid: %appdata%\Microsoft\teams\tmp.

    4. Taaskäivitage oma Teamsi klient.
