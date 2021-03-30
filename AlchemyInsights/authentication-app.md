---
title: Autentimisrakendus
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404599"
---
# <a name="authentication-app"></a>Autentimisrakendus

Kui olete üldadministraator, saate sisselogimisdiagnostika abil kiiresti teada saada, mis juhtus või diagnoosida kasutaja [sisselogimisega seotud probleeme.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Käivitage diagnostika, klõpsates nuppu["Käivita diagnostika".](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom) 
1. Uurige analüüsitav sündmus, sisestades kasutaja, rakenduse, sisselogimisaja, päringu ID või korrelatsiooni ID üksikasjad.
1. Vaadake üle diagnostikatulemid, kus on kuvatud üksikasjad selle kohta, mis juhtus ja milliseid toiminguid saate muudatuste vaatamiseks teha ( kui on vaja teha muudatusi).

**Kontrollige, mis on rakendatav.**

1. Kui kasutaja ei saa rakenduses Microsoft Authenticator tõuketeatist, veenduge, et neid ei kuvata MFA blokeeritud kasutajate all, nagu on kirjeldatud jaotises Kasutajate [blokeerimine ja blokeeringu blokeerimine.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
1. Kui kasutaja ei blokeeri MFA-d, kuid ei saa tõuketeatist, saab ta avada Rakenduse Microsoft Authenticator, mis võtab ootel kinnitamise taotlused.
1. Alternatiivse sisselogimisviisina saab kasutaja klõpsata ka nuppu Logi sisse muul viisil ja valida mobiilirakenduse kinnituskoodi.
1. Microsoft Authenticatori rakendus on ainus saadaval meetod paljude kasutajate jaoks. [Lugege lisateavet turbe vaikesätete kohta,](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)vaadake [korduma kippuvate](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) küsimuste ja nende lahendamise kohta authenticatori rakenduse KKK-d.
 
**Soovitatavad videod**

[Authenticatori rakenduse häälestamine uues telefonis (2min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
