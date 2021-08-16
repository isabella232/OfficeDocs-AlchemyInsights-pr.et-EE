---
title: Logid ja aruandlus
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004331"
- "7727"
ms.openlocfilehash: 03d77c17622a1aac5ecb035bb5b73efdbbfe5e6b141e6b266eef8783f612c8b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067008"
---
# <a name="logs-and-reporting"></a>Logid ja aruandlus

[Azure Active Directory kkk vastab](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) korduma kippuvatele küsimustele Azure Active Directory (Azure AD) aruandluse kohta. Lisateavet leiate teemast [Azure Active Directory aruandlus](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).

**Auditiga seotud probleemide tõrkeotsing**

1. Kui teil on probleeme mõne audititegevuse nägemisega ja loendis puudub [tegevus,](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)esitage tugipilet.
2. Kui teil on probleeme rentnikus auditilogide nägemisega, esitage tugipilet.
3. Kui teie audititegevusi ei kuvata Azure'i portaalis kohe, vaadake meie latentsusteavet ja kui viivitus ületab dokumenteeritud latentsusruumi, saate esitada tugipileti. [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies)
4. [Azure AD tegevuslogide säilitamine](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. Kui te ei näe valitud kuupäevavahemiku auditit, saate Azure'i portaalist alla laadida kuni 250 K rida (sorditud uusimate järgi). Lisateavet leiate teemast [Audititegevuste allalaadimine.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report)

**Sisselogimisprobleemide tõrkeotsing**

1. Viimase 30 päeva andmeid saate vaadata ainult siis, kui teil on rentniku jaoks Azure AD Premium (P1 või P2) litsents.
2. Sisselogimisi saab kasutada ainult Azure AD Premium rentnike jaoks. See pole saadaval tasuta või põhilitsentsitud rentnike jaoks.
3. Kui teie rentnikul on Premium P1-litsents ja te ei näe sisselogimisi, vaadake meie latentsusteavet ja kirjutage tugipilet, kui viivitus ületab dokumenteeritud latentsusaja. [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies)
4. Kui te ei näe kõiki valitud kuupäevavahemiku sisselogimisi, võtke arvesse, et azure'i portaalist saate alla laadida kuni 250 K rida (sorditud uusimate järgi). Lisateavet leiate teemast [Sisselogimistegevuste allalaadimine.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities)

**Turbearuannete tõrkeotsing (ohuga lipuga märgitud kasutajad, riskantne sisselogimine)**

1. [Riskiturbearuande lipuga märgitud kasutajad](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [Riskantne sisselogimisaruanne Azure Active Directory portaalis](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [Azure Active Directory riskisündmused](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
