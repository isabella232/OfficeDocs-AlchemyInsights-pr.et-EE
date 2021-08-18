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
ms.openlocfilehash: 97a8d4e7db9aac65e6a505c0bef8b41d2ea23353
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323914"
---
# <a name="configure-endpoint-dlp"></a>Lõppseadmete andmelekketõkestuse konfigureerimine

Microsofti lõppseadmete andmelekketõkestuse funktsioon lubab teil DLP kaitset ja seirevõimalusi laiendada ka Windows 10 seadmetes leiduvale delikaatsele teabele. Pärast seda, kui seadmed on seadmehalduses registreeritud, saate luua DLP-poliitikad üksustega tehtavate kaitsetoimingute jõustamiseks. Tegevuse-uurijat saab kasutada tegevuste kontrollimiseks delikaatse teabe asjus. Lisateavet leiate artiklist [Seadmete kasutuselevõtt seadmehalduses](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Lõppseadmete andmelekketõkestuse kasutuselevõtuks tehke järgmist.

- Veenduge, et teil oleks asjakohaste SKU-de / tellimuste litsentsid. Lisateavet leiate artiklist [SKU-de / tellimuste litsentsid](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Kontrollige üle seadmehalduse lubamise, kasutuselevõtulehele juurdepääsu või seadmeseire sisse- ja väljalülitamise õigused. Lisateavet leiate artiklist [Õigused](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Seadmete kasutuselevõtuks seadmehalduses täitke seadmete kasutuselevõtu juhised. Lisateavet leiate artiklist [Seadmete kasutuselevõtt](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Delikaatsete üksuste kaitsmiseks looge DLP-poliitikad. Lisateavet leiate artiklist [Lõppseadmete andmelekketõkestuse poliitika stsenaariumid](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

Lisateavet Microsofti lõppseadmete andmelekketõkestuse kohta leiate artiklist [Microsoft 365 lõppseadmete andmelekketõkestuse (eelversioon) teave](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Olulised andmete kogumise juhised, kui vaja on kasutajatuge**

1. Laadige [alla MDATP kliendi analüsaatori eelvaade.](https://aka.ms/betamdatpanalyzer)
1. Käivitage tööriist administraatorina käsuviibaaknas:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Kui kuvatakse teade **Sisestage jälituste** kogumiseks minutite arv: sisestage stsenaariumi käivitamiseks vajalik minutite arv.
1. Käivitage stsenaarium.

Koguge zip-faili väljund tugiagendile andmiseks.
