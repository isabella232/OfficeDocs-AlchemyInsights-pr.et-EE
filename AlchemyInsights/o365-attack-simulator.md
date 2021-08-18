---
title: 2681 Attack Simulator Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: f6e221cc82a1b707f6acc457cb78db743521d859
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325067"
---
# <a name="attack-simulator-in-microsoft-365"></a>Attack Simulator in Microsoft 365

- Kas teil puudub ründesimulaator? Ründesimulaatori **kasutamiseks on vaja Microsoft Defenderit Office 365 2.** või Office 365 Enterprise **E5 jaoks.** **Ründesimulaatorit ei** kaasata Microsoft Defenderi Office 365 1, Office 365 Enterprise E3 ega Microsoft 365 ettevõtterakendused tellimuste jaoks.

- Simuleeritud rünnakute käivitamiseks kasutav konto nõuab üldadministraatori või turbeadministraatori õigusi ja mitme teguriga autentimist (MFA). Lisateavet ründesimulaatori nõuete kohta leiate [sellest teemast.](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)

- Oluline teave **Brute Force Passwordi rünnaku simulatsioonide** kohta.

  - Kui sihtkontol on lubatud MFA ja parool arvati õigesti ära, ei kuvata kontot ohustatud kontona (teine autentimistegur pole täielik).

  - Paroolifail ei tohi olla suurem kui 10 MB. Kasutage ühte parooli rea kohta ja lisage loendis viimase parooli järele tühi rida (tagasijooksu).

- Olulised asjad, mida saate **teada oda andmepüügist, kinnitage** simulatsioonid.

  - Vaikimisi ei saa andmepüügilogimisserveri URL-i jaoks **kohandatud väärtust sisestada.**

  - Kui adressaat kasutab [](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) sõnumi andmepüügiks teatamiseks lisandmoodulit Teata sõnumist, ei pruugi te sõnumi kohta teatisi vastu võtta (kuna see on simuleeritud rünnak).

- Aruanded. Pärast simuleeritud rünnaku lõpule viimist saate aruande **koostamiseks** klõpsata nuppu Rünnaku üksikasjad.

- Üksikasjalikud juhised ja uued funktsioonid ründesimulaatoris leiate teemast [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
