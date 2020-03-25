---
title: SharePointi migreerimise ahendamine 503 tõrked
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931654"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a>SharePointi migreerimise ahendamine 503 tõrked

**Oluline**: paljud SharePoint Online ' i ja OneDrive kliendid käivitada Business kriitilised rakendused teenuse, mis töötavad taustal. Nende hulka kuuluvad sisu migratsioon, andmete kadu vältimine (DLP) ja backup lahendused. Nendel enneolematul ajal me võtame meetmeid, et tagada SharePoint Online ' i ja OneDrive teenused on väga kättesaadav ja usaldusväärne oma kasutajatele, kes sõltuvad teenuse rohkem kui kunagi varem kaugtöö stsenaariume.

Selle eesmärgi toetuseks oleme rakendanud ranget ahendamise piiranguid taustal olevatele rakendustele (migratsioon, DLP ja backup lahendused) tööpäeval päeva jooksul. Te peaksite ootama, et need rakendused saavutavad nende aegade jooksul väga piiratud läbilaskevõime. Aga, õhtuti ja nädalavahetusel tundi piirkonna, teenus on valmis töötlema oluliselt suurem hulk taotlusi taustal apps.

**503 tõrked, kui migreerimine SharePoint Online**

Tundub, et migreerite SharePoint Online ' i ja saate 503 tõrked. Palun järgige alltoodud samme, et saaksime teid aidata nii ruttu kui võimalik. 

1. Klõpsake nuppu **Kontakt tugiteenja**seejärel **uue teenuse taotlus**.
2. Pealkirja ja kirjeldus, tippige **SharePointi migreerimise ahendamine koos 503**.
3. Kui pilet on esitatud, värskendage seda järgmise teabega:
    - Kui palju jäänud migratsioon (näiteks kui palju TBs?).
    - Migratsiooni algus-ja lõppkuupäev.
    - Kirjeldage, kus olete oma sisu migreerimine (nt SharePoint Server, kast, GDrive, failide osad jne).
    - Kas hinnata ahendamisvigade arvu (nt x-Throttle tunnis?) ja millal see ahendamine juhtus.
    - Millist siirdustööriista kasutate (nt SPMT või ShareGate).


