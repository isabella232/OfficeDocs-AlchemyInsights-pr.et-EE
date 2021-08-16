---
title: Tingimusjuurdepääsu probleemid
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
ms.openlocfilehash: 85cbd89e461f36a51eed816619fd132ea60dfdb0014eb850c7ec3f38d41e1ca2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069960"
---
# <a name="conditional-access-issues"></a>Tingimusjuurdepääsu probleemid

**Sisselogimisdiagnostika probleemide lahendamine**

Sisselogimisdiagnostika abil saate kiiresti teada, mis juhtus või diagnoosida kasutaja [sisselogimisega seotud probleeme.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Käivitage sisselogimisdiagnostika.
1. Uurige analüüsitav sündmus, sisestades kasutaja, rakenduse, sisselogimisaja, päringu ID või korrelatsiooni ID üksikasjad.
1. Vaadake üle diagnostikatulemid, kus on kuvatud üksikasjad selle kohta, mis juhtus ja milliseid toiminguid saate muudatuste vaatamiseks teha (kui on vaja teha muudatusi).

**Juhised sisselogimise tõrkeotsinguks** 

1. Liikuge Azure AD sisselogimislehele.
1. Filtreerige sisselogimisi kasutaja, ajavahemiku, rakenduse, oleku, klientrakenduse jne järgi.
1. Valige sisselogimissündmus ja vaadake vahekaarti Tingimusjuurdepääs, et näha, milliseid poliitikaid on hinnatud.
1. Poliitika üksikasjade kuvamiseks ja selle rakendamis põhjuste vaatamiseks klõpsake poliitikarida.

**Tingimusjuurdepääsu poliitika tõrkeotsingu tööriistad**

- Ainult aruanderežiim võimaldab teil poliitikat hinnata ilma kasutajaid mõjutamata.
- What-if tool võimaldab teil simuleerida sisselogimissündmusi ja vaadata, millised poliitikad kehtivad.
- Ülevaated ja aruandlustöövihik kuvab iga poliitika reaalajas mõju.

**Baseline Protection Policies**

Baseline Protection policies on aegunud. Neid ei jõustata enam ja need eemaldatakse peagi Azure'i portaalist. Soovitame lubada [turbe vaikesätted.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)

Lisateavet tingimusjuurdepääsu kohta leiate teemast

[Tingimusjuurdepääsu head tavad Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Tingimusjuurdepääsu tingimused](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Tingimusjuurdepääsu juhtelemendid](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Tingimusjuurdepääsu asukohad](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
