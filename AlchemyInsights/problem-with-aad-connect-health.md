---
title: Probleem AAD Connecti tervisega
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481465"
---
# <a name="problem-with-aad-connect-health"></a>Probleem AAD Connecti tervisega

- Veenduge, et teil on toimingu tegemiseks õigus. Globaalsetel administraatoritel on vaikimisi juurdepääs. Lisaks saate kasutada [rolli baasil juurdepääsu juhtelementi](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) , et anda delegaadile registreerimise õigused.
- Veenduge, et nõutavad lõpp-punktid on lubatud ja tulemüüri tõttu blokeeritud. Lisateavet leiate teemast [nõuded](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Registreerimine võib nurjuda tänu sellele, et võrgu kiht teostab väljaminevat suhtlust SSL-i kaudu.
- Veenduge, et olete Azure AD Connecti tervise teatiste sätteid kinnitanud. Vaadake oma säte üle. See [juhend](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) aitab teil aru saada, kuidas KONFIGUREERIDA Azure AD Notificationi teatiste sätteid.
- Lisateavet AAD Connecti Health Synci aruannete ja selle allalaadimise kohta leiate teemast [objekti taseme sünkroonimise teatis](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Kui soovite, et AAD Connect Healthi teatised, järgige juhiseid, mis [on esitatud jaotises AAD ühenduse tervise andmete värskuse teatiste](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) ja korduma kippuvate küsimuste kohta leiate teavet teemast [Üldine AAD Connect Health Installation](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
