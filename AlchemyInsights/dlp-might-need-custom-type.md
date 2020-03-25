---
title: DLP võib vajada kohandatud tüüpi
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932654"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP võib vajada kohandatud tüüpi

**Oluline**: paljud SharePoint Online ' i ja OneDrive kliendid käivitada Business kriitilised rakendused teenuse, mis töötavad taustal. Nende hulka kuuluvad sisu migratsioon, andmete kadu vältimine (DLP) ja backup lahendused. Nendel enneolematul ajal me võtame meetmeid, et tagada SharePoint Online ' i ja OneDrive teenused on väga kättesaadav ja usaldusväärne oma kasutajatele, kes sõltuvad teenuse rohkem kui kunagi varem kaugtöö stsenaariume.

Selle eesmärgi toetuseks oleme rakendanud ranget ahendamise piiranguid taustal olevatele rakendustele (migratsioon, DLP ja backup lahendused) tööpäeval päeva jooksul. Te peaksite ootama, et need rakendused saavutavad nende aegade jooksul väga piiratud läbilaskevõime. Aga, õhtuti ja nädalavahetusel tundi piirkonna, teenus on valmis töötlema oluliselt suurem hulk taotlusi taustal apps.

**DLP võib nõuda kohandatud teabe tüüp**

Andmete kadu vältimine (DLP) poliitika, saate tuvastada ja kaitsta tundliku loomuga andmeid oma organisatsioonis. Mõnel juhul peate võib-olla looma oma **kohandatud** tundliku teabe tüübi, et kaitsta oma organisatsiooni andmeid.

Näiteks võib teie organisatsioonil olla vaja tuvastada ja kaitsta töötaja ID-sid või muid andmeid mõnes teie organisatsioonile eriomas vormingus. Kui jah, lugege lisateabe saamiseks järgmisi artikleid.
  
 **Sisseehitatud tundliku teabe tüübi kohandamine**
  
Kui sisseehitatud tundlik teabetüüp rahuldaks teie vajadused vaid mõne tweaks, saate [kohandada sisseehitatud tundliku teabe tüüpi](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type). Näiteks saate märksõnu lisada või eemaldada või lisada või eemaldada täiendavaid tõendeid (nt kuupäev või aadress).
  
 **Kohandatud tundliku teabe tüübi loomine**
  
Kuid kui teil on vaja tuvastada ja kaitsta erinevat tüüpi tundlikku teavet, saate [luua kohandatud tundliku teabe tüübi](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) Security & vastavuse keskus UI.
  
**Luua kohandatud tundliku teabe tüüp Security & vastavuse keskus PowerShelli**

Lõpuks, kui UI ei paku kõik vajalikud suvandid, saate [luua kohandatud tundliku teabe tüüp Security & vastavuse keskus PowerShelli](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell). Alustades XML-failist, saate kasutada igat saadaolevat suvandit.
