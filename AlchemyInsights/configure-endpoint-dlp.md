---
title: Lõppseadmete andmelekketõkestuse konfigureerimine
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402416"
---
# <a name="configure-endpoint-dlp"></a>Lõppseadmete andmelekketõkestuse konfigureerimine

Microsofti lõppseadmete andmelekketõkestuse funktsioon lubab teil DLP kaitset ja seirevõimalusi laiendada ka Windows 10 seadmetes leiduvale delikaatsele teabele. Pärast seda, kui seadmed on seadmehalduses registreeritud, saate luua DLP-poliitikad üksustega tehtavate kaitsetoimingute jõustamiseks. Tegevuse-uurijat saab kasutada tegevuste kontrollimiseks delikaatse teabe asjus. Lisateavet leiate artiklist [Seadmete kasutuselevõtt seadmehalduses](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Lõppseadmete andmelekketõkestuse kasutuselevõtuks tehke järgmist.

- Veenduge, et teil oleks asjakohaste SKU-de / tellimuste litsentsid. Lisateavet leiate artiklist [SKU-de / tellimuste litsentsid](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Kontrollige üle seadmehalduse lubamise, kasutuselevõtulehele juurdepääsu või seadmeseire sisse- ja väljalülitamise õigused. Lisateavet leiate artiklist [Õigused](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Seadmete kasutuselevõtuks seadmehalduses täitke seadmete kasutuselevõtu juhised. Kui te ei näe M365 vastavuskeskuse jaotises **Sätted** seadmete kasutuselevõtu (eelversiooni) sätet, siis veenduge, et teil oleksid olemas eespool viidatud vajalikud litsentsid ja õigused. Lisateavet leiate artiklist [Seadmete kasutuselevõtt](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Delikaatsete üksuste kaitsmiseks looge DLP-poliitikad. Lisateavet leiate artiklist [Lõppseadmete andmelekketõkestuse poliitika stsenaariumid](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).

Lisateavet Microsofti lõppseadmete andmelekketõkestuse kohta leiate artiklist [Microsoft 365 lõppseadmete andmelekketõkestuse (eelversioon) teave](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Olulised andmete kogumise juhised, kui vaja on kasutajatuge**

1. Laadige siit alla MDATP Client Analyzeri eelversioon: [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer").
2. Käivitage tööriist administraatorina käsuviibaaknas:
3. MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t
4. Kui teil palutakse sisestada jälitusteabe kogumise kestus minututes, sisestage stsenaariumi käitamiseks vajalik aeg minutites.
5. Käivitage stsenaarium.

Koguge tugiagendile edastamiseks vajalik väljund-ZIP-fail.
