---
title: E-juurdluse tõrkeotsing sisaldab tõrkeid
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676147"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>E-juurdluse tõrkeotsing sisaldab tõrkeid

Kas teil on probleeme e-juurdlusega? Siin on mõned head tavad, mida kaaluda.

- Kontrollige ootel jaotusolekut.  Kui olek **on Sees (Ootel) või** Väljas **(Ootel),** oodake, kuni ootel jaotus on lõpule viidud.
- E-juurdluse värskenduste ühendamine ühekordse hulgitaotlusena, mitte iga tehingu poliitika korduva värskendamise asemel.
- Käivitage Set-CaseHoldPolicy <policyname> -RetryDistribution turbe- ja vastavuskeskuse PowerShellis. Lisateavet leiate teemast [Ühendus Security & PowerShell](/powershell/exchange/connect-to-scc-powershell).

Nende sätete ja täiendavate e-juurdluse leevendamise ja lahendamise parimate tavade kontrolli juhised leiate teemast [E-juurdluse ootel](/microsoft-365/compliance/hold-distribution-errors)oleku tõrgete tõrkeotsing.
Lisateavet muude levinud e-juurdluse probleemide tõrkeotsingu kohta leiate teemast [Levinuma](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)e-juurdluse probleemide juurdlus, tõrkeotsing ja lahendamine.
