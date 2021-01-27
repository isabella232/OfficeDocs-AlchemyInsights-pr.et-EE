---
title: Tingimuslikud Accessi probleemid
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014788"
---
# <a name="conditional-access-issues"></a>Tingimuslikud Accessi probleemid

**Sisselogimise diagnostikaga seotud probleemide lahendamine**

[Sisselogimise diagnostika](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)abil saate kiiresti teada, mis juhtus kasutaja sisselogimisega seotud probleemide või diagnoosimisega.

1. Käivitage sisselogimise diagnostika.
1. Analüüsitud sündmuse otsimine, sisestades andmed, mis teil on kasutaja, rakenduse, sisselogimise aja, päringu ID või korrelatsiooni ID-ga.
1. Vaadake üle diagnostilised tulemid, mis näitavad üksikasju juhtunu kohta ja milliseid toiminguid saab teha muudatuste tegemiseks (kui on vaja muudatusi teha).

**Sisselogimise tõrkeotsingu toimingud** 

1. Liikuge lehele Azure AD sign-in.
1. Filtreerige sisselogimisi kasutaja, ajavahemikus, rakendus, olek, klientrakendus jne.
1. Valige sisselogimise sündmus ja vaadake vahekaarti tingimusjuurdepääsu, et näha, milliseid poliitikaid hinnati.
1. Poliitika üksikasjade kuvamiseks klõpsake poliitika rida ja saage aru, miks see rakendati.

**Tööriistad tingimusliku juurdepääsu poliitika tõrkeotsinguks**

- Ainult aruandlusega režiimis saate poliitikaid hinnata, mõjutamata kasutajaid.
- Mis-tööriista abil saate simuleerida sisselogimise sündmusi ja vaadata, millist poliitikat kohaldatakse.
- Ülevaadete ja aruannete töövihik kuvab iga poliitika reaalajas mõju.

**Baseline Protection poliitika**

Baseline Protection poliitika on aegunud. Neid ei rakendata enam ja see eemaldatakse peagi Azure ' i portaalist. Soovitame [turvalisuse vaikesätteid](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)lubada.

Lisateavet tingimusliku juurdepääsu kohta leiate järgmistest teemadest.

[Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 tingimusliku juurdepääsu parimad tavad [Tingimustega tingimusjuurdepääsu tingimused](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Juhtelementide kasutamine](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 tingimusjuurdepääsu korral [Asukohad tingimusjuurdepääsu kaudu](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
