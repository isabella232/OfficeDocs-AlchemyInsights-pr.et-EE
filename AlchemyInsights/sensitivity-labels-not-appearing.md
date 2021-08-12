---
title: Tundlikkussilte ei kuvata
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 824824257fee4aaaab1f2dd32597b4cdc858d035fabd357af90cf054dd35c9c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061428"
---
# <a name="sensitivity-labels-not-appearing"></a>Tundlikkussilte ei kuvata

Tundlikkussildid võimaldavad teil tundliku sisu liigitada ja kaitsta. Neid saab luua Microsoft 365 vastavuskeskus, Microsoft 365 turbekeskuses või Microsoft 365 & jaotises Tundlikkussildid > turbekeskuses. Lisateavet selle funktsiooni kohta leiate teemast [Tundlikkussiltide ülevaade](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

Kui konfigureerite oma tundlikkussildid, kuid neid ei kuvata Microsoft 365 rakendustes, kontrollige järgmist.

- Veenduge, et tundlikkuse silt [on avaldatud](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) soovitud kasutajatele ja rühmadele.

- Veenduge, et kasutaja kasutab rakendust, mis toetab tundlikkussilte – vt [dokumendi tundlikkussilte.](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable)

- Kui migreerite [Azure'i teabekaitse silte,](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)arvestage siin loetletud [kaalutlustega.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)

- Andmekao vältimise (DLP) tugi. Praegu saab DLP-poliitikates tingimusena kasutada ainult säilitussilte.  Tundlikkussiltide tugi DLP-poliitikas pole veel saadaval, kuid me töötame selle kallal.

- Kui krüptimine on tundlikkussildil lubatud, saate valida ühe järgmistest.
    - Õiguste määramine kohe
    - Luba kasutajatel õigusi määrata


Lisateavet võimalike probleemide kohta leiate teemast [Teadaolevad probleemid tundlikkussiltide abil.](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)