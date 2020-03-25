---
title: DLP ei tööta ootuspäraselt
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932618"
---
# <a name="dlp-not-working-as-expected"></a>DLP ei tööta ootuspäraselt

**Oluline**: paljud SharePoint Online ' i ja OneDrive kliendid käivitada Business kriitilised rakendused teenuse, mis töötavad taustal. Nende hulka kuuluvad sisu migratsioon, andmete kadu vältimine (DLP) ja backup lahendused. Nendel enneolematul ajal me võtame meetmeid, et tagada SharePoint Online ' i ja OneDrive teenused on väga kättesaadav ja usaldusväärne oma kasutajatele, kes sõltuvad teenuse rohkem kui kunagi varem kaugtöö stsenaariume.

Selle eesmärgi toetuseks oleme rakendanud ranget ahendamise piiranguid taustal olevatele rakendustele (migratsioon, DLP ja backup lahendused) tööpäeval päeva jooksul. Te peaksite ootama, et need rakendused saavutavad nende aegade jooksul väga piiratud läbilaskevõime. Aga, õhtuti ja nädalavahetusel tundi piirkonna, teenus on valmis töötlema oluliselt suurem hulk taotlusi taustal apps.

 **DLP seadistamine**

Kas teil on probleeme **andmete kadu vältimine (DLP)** Office 365 ei tööta ootuspäraselt? Kui jah, veenduge, et teie **DLP poliitika** on õigesti seadistatud ja et teie andmed sisaldavad seda, mida **DLP poliitika** otsib, kui seda hinnatakse.
  
DLP poliitika võimaldab teil tuvastada ja kaitsta tundliku loomuga teavet oma organisatsioonis. DLP poliitikate häälestamise puhul kasutage [siin](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)olevat teavet.
  
 **Mida DLP poliitikad otsida**
  
**Sisseehitatud tundliku teabe tüüpide** kasutamisel Office 365 turvalisuse ja vastavuse keskus, DLP poliitika otsida konkreetseid mustreid ja elemente, kui need tundlikud tüübid tuvastada.
  
- **Sisseehitatud tundlikud teabetüübid**

    Teave sisseehitatud tundlik tüübid ja mida DLP poliitika otsib kui tuvastamine tundlik tüüp, vaadake: [mida tundliku teabe tüübid otsida](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- **Kohandatud tundliku teabe tüübid**

    Kui proovite luua kohandatud tundliku teabe tüüpe, kasutage järgmist artiklit teabe saamiseks kohandatud tundliku tüübi loomise kohta: [kohandatud tundliku teabe tüübi loomine](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).

**DLP poliitika testimine**

Oma andmete testimiseks sisseehitatud või kohandatud tundliku teabe tüübiga kasutage suvandit **testi tüüp jaotises liigitustundlikud** **Classifications** > **teabetüübid**. Lisateabe saamiseks vt teemat [kohandatud tundliku teabe tüüpide testimine](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).

 **Aruanded**
  
- Hankige tundlikud andmete ülevaated [DLP aruannetega.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)

- Vaadake juhtumi konkreetseid üksikasju [intsidendi aruandega](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).
