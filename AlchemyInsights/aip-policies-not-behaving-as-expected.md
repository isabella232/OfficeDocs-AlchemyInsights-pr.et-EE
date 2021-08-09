---
title: 'AIP: poliitikad ei käitu ootuspäraselt'
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
- "4780"
ms.openlocfilehash: 90448bf57297ce59ba222efd1927b5de588bfbfdb1206b6403764d7f43fed690
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934289"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: poliitikad ei käitu ootuspäraselt

Azure'i teabekaitse: poliitikad ei käitu ootuspäraselt, erinevate poliitikaprobleemide kohta leiate järgmisi juhiseid.

1. Kui teil on visuaalse märgistusega probleeme, vaadake üle, [kui rakendatakse visuaalseid märgistusi.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. Kui teil on probleeme automaatse sildistusfunktsiooniga, lugege teemat Kuidas konfigureerida [Azure'i](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) teabekaitse automaatse ja soovitatava liigituse tingimusi ja mida tundliku [loomuga teabetüübid pakuvad.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
3. Kui teil on probleeme native/Pfile'i kaitsega, vaadake üle faili [API konfiguratsioon.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)
4. Kontrollige, kas kasutate ulatusega poliitikaid, mis pole õigesti konfigureeritud: Azure'i teabekaitsepoliitika konfigureerimine kindlate kasutajate jaoks [ulatusega poliitikate abil.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
5. Kui automaatne sildistamine ei tööta sildistatud dokumendi Outlook, veenduge, et DRMEncryptProperty pole määratletud järgmiselt: [IRM-i registrisätted turbe jaoks.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)

Kui teil esineb endiselt probleeme, koguge Azure'i teabekaitse kliendi logid ja manustage eksporditud logid sellele piletile.

1. Avage Office või looge uus meilisõnum Outlook.
2. Klõpsake **nuppu Kaitse/tundlikkuse**  >  **spikker ja tagasiside.**
3. Klõpsake **nuppu Ekspordi logid.**
4. Salvestage logid oma asukohavalikusse ja manustage need sellele teenusetaotlusele.

Lisaressursid:

- [Azure'i teabekaitse jaoks visuaalsete märgistuste sildi konfigureerimine](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Azure'i teabekaitse dokumentatsiooni läbivaatamine](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Tundlikkussiltide kasutamine Microsoft 365 rakendustes](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

