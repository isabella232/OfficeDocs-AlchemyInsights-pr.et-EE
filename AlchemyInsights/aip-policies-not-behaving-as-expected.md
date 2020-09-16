---
title: 'AIP: poliitika ei käitu ootuspäraselt'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663185"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: poliitika ei käitu ootuspäraselt

Azure ' i teabe kaitse: poliitikad, mis ei toimi ootuspäraselt, leiate järgmistest teemast Soovitatavad juhised.

1. Kui teil on probleeme visuaalse märgistusega, vaadake [visuaalse märgistuse rakendamisel](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Kui teil on automaatse sildistamisega probleeme, vaadake, [Kuidas konfigureerida Azure ' i teabe kaitse automaatse ja soovitatava klassifikatsiooni tingimusi](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) ning [milliseid tundlikke teabe tüüpe otsida](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Kui teil on emakeelena/Pfile kaitsega probleeme, vaadake läbi selle [API konfiguratsioon](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Kontrollige, kas kasutate ulatusega poliitikaid, mida pole õigesti konfigureeritud: [Kuidas konfigureerida Azure ' i teabe kaitsmise poliitika kindlate kasutajate jaoks ulatusega poliitikate abil](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Kui siltidega dokumendi manustamisel ei tööta automaatne sildistamine Outlooki jaoks, veenduge, et DRMEncryptProperty poleks määratletud, nagu on kirjeldatud siin: [turbe IRM-i registrisätete sätted](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Kui teil esineb endiselt probleeme, palume koguda Azure ' i teabeõiguste kaitse kliendi logisid ja lisada eksporditud logid sellele pilet.

1. Avage Office ' i dokument või looge Outlookis Uus meilisõnum.
2. Klõpsake nuppu **kaitse/tundlikkuse**  >  **Spikker ja tagasiside**.
3. Klõpsake nuppu **ekspordi logid**.
4. Salvestage logid oma asukoha valikusse ja lisage need selle teenuse taotlusele.

Lisaressursid:

- [Azure ' i teabe kaitsmiseks mõeldud visuaalsete märkide sildi konfigureerimine](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Azure ' i teabe kaitse dokumentatsiooni läbivaatamine](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Microsoft 365 rakenduste tundlikkuse siltide kasutamine](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

