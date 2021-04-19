---
title: Automaatne liigitus ei käitu AIP-klientrakenduses ootuspäraselt
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4373"
ms.openlocfilehash: b7ab09fe8430a54dacf2cd1ba076414a5f562541
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820894"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Automaatne liigitus ei käitu AIP-klientrakenduses ootuspäraselt

Automaatne liigitus ei käitu ootuspäraselt, kasutage järgmisi soovitatavaid juhiseid.

1. Kui teil on probleeme automaatse sildistusfunktsiooniga, lugege teemat [Azure'i](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) teabekaitse automaatse ja soovitatava liigituse tingimuste konfigureerimine ja Tundliku [sisuga teabetüüpide konfigureerimine.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
2. Kontrollige, kas kasutate ulatusega poliitikaid, mis pole õigesti konfigureeritud: Azure'i teabekaitsepoliitika konfigureerimine kindlate kasutajate jaoks [ulatusega poliitikate abil.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
3. Kui sildistatud dokumendi manustamise korral ei tööta Outlookis automaatne sildistamine, veenduge, et see poleks määratletud `DRMEncryptProperty` järgmiselt: [IRM-i registrisätted turbe jaoks.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)
4. Kui kasutasite [Azure'i teabekaitse poliitika](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) jaoks sisseehitatud teabetüüpe, veenduge, et teie sisu vastaks eeldatud vormingule.
5. Veenduge, et silt oleks õigesti konfigureeritud automaatseks **või** **soovitatavaks.** (**Automaatne** sildistamine on saadaval kõigi Microsoft 365 rakenduste jaoks, soovitatav on saadaval kõigi Microsoft 365 rakenduste jaoks peale Outlooki.) 
6. Automaatset liigitust ei saa kasutada dokumentide ja meilisõnumite puhul, mis olid varem käsitsi sildistatud või varem automaatselt märgistatud kõrgema liigitusega.  Lisateavet leiate teemast Automaatsete [või soovitatavate siltide kasutamine.](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied)
7. Kui teil esineb endiselt probleeme, koguge Azure'i teabekaitse kliendilogid ja manustage eksporditud logid oma tugiteenuste piletile. Azure'i teabekaitse logide eksportimiseks:
    - Avage Office'i dokument või looge Outlookis uus meilisõnum.
    - Klõpsake **nuppu Kaitse/tundlikkuse**  >  **spikker ja tagasiside.**
    - Klõpsake **nuppu Ekspordi logid.**
    - Salvestage logid oma asukohavalikusse ja manustage need oma teenusetaotlusele.

Lisateavet leiate teemast

- [Azure'i teabekaitse automaatse ja soovitatava liigituse tingimuste konfigureerimine](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Juhised Azure'i teabekaitset kasutav tavastsenaarium](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Azure'i teabekaitse dokumentatsiooni läbivaatamine](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Azure'i teabekaitse tellimuste ja funktsioonide läbivaatamine](https://azure.microsoft.com/pricing/details/information-protection)
- [Azure'i teabekaitse nõuded](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Azure'i teabekaitse lühikäivitusõpetus](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Azure'i teabekaitse kliendi allalaadimine](https://www.microsoft.com/download/details.aspx?id=53018)
