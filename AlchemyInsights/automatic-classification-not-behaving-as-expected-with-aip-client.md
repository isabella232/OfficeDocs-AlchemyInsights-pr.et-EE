---
title: Automaatne klassifikatsioon ei käitudes AIP kliendiga ootuspäraselt
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4373"
ms.openlocfilehash: 22eeb6ba32e4e943efa2495a477ff394f3c135db
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508372"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Automaatne klassifikatsioon ei käitudes AIP kliendiga ootuspäraselt

Automaatne klassifikatsioon ei käitudes ootuspäraselt, kasutage järgmisi soovituslikke juhiseid:

1. Kui teil on probleeme automaatse märgistamise, vaadake, [Kuidas konfigureerida tingimused automaatne ja soovitatav klassifikatsioon Azure ' i teabekaitse](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) ja [mida tundliku teabe tüübid otsida](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Kontrollige, kas kasutate hõlmavaid poliitikaid, mis pole õigesti konfigureeritud: [Kuidas konfigureerida Azure ' i teabe kaitse poliitika teatud kasutajatele, kasutades ulatatud poliitikad](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Kui automaatne märgistamine ei tööta Outlooki sildistatud dokumendi ühendamisel, veenduge, et `DRMEncryptProperty` pole määratletud siin kirjeldatud: [IRM registrisätted turvalisuse](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Kui kasutasite oma Azure ' i teabekaitse poliitika [sisseehitatud teabetüüpe](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) , veenduge, et teie sisu vastaks eeldatava vorminguga.
5. Veenduge, et silt oleks sobivalt konfigureeritud **automaatseks** või **soovitatavaks**. (**Automaatne** märgistamine on saadaval kõigi Office ' i rakenduste jaoks, samas kui **soovitatav** on kasutada kõiki Office ' i rakendusi peale Outlooki.)
6. Te ei saa kasutada automaatset liigitust dokumentidele ja e-kirjadele, mis olid varem käsitsi märgistatud või varem automaatselt märgistatud kõrgema klassifikatsiooniga.  Lisateabe saamiseks vaadake: [Kuidas rakendatakse automaatselt või soovitatud silte](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Kui teil on endiselt probleeme, palun koguda Azure ' i teabe kaitse kliendi logid ja kinnitage eksporditud logid oma tugiteenuse pilet. Azure ' i teabekaitse logid eksportimiseks toimige järgmiselt.
    - Avage Office ' i dokument või looge Outlookis uus e-kiri.
    - Klõpsake valikul **kaitse/tundlikkuse**  >  **Spikker ja tagasiside**.
    - Klikkige käsul **ekspordi logid**.
    - Salvestage logid oma asukoha valikule ja kinnitage need oma teenustaotlusele.

Lisateavet leiate teemast:

- [Kuidas konfigureerida automaatse ja soovitatava klassifikatsiooni Azure ' i teabe kaitse tingimused](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Kuidas-juhised levinud stsenaariumid, mis kasutavad Azure ' i teabekaitse](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Azure ' i teabekaitse dokumentatsiooni läbivaatamine](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Vaadake üle Azure ' i teabekaitse tellimused ja funktsioonid](https://azure.microsoft.com/pricing/details/information-protection)
- [Azure ' i teabekaitse nõuded](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Quick Start juhendaja Azure ' i teabekaitse](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Laadige alla Azure ' i teabekaitse klient](https://www.microsoft.com/download/details.aspx?id=53018)
