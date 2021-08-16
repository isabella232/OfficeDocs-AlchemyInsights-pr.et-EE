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
ms.openlocfilehash: b173c6eb3bbbd1beba3b59878ae12bbe7684d0447a16fef746e5b97b82349e53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065280"
---
# <a name="attack-simulator-in-microsoft-365"></a>Attack Simulator Microsoft 365

- Kas teil puudub ründesimulaator? Ründesimulaatori **kasutamiseks on vaja Microsoft Defenderit Office 365 2** või Office 365 Enterprise **E5 jaoks.** **Ründesimulaatorit ei** kaasata Microsoft Defenderi Office 365 1, Office 365 Enterprise E3 ega Microsoft 365 ettevõtterakendused tellimuste jaoks.

- Simuleeritud rünnakute käivitamiseks kasutav konto nõuab üldadministraatori või turbeadministraatori õigusi ja mitme teguriga autentimist (MFA). Lisateavet ründesimulaatori nõuete kohta leiate [sellest teemast.](/microsoft-365/security/office-365-security/attack-simulator)

- Oluline teave **Brute Force Passwordi rünnaku simulatsioonide** kohta.

  - Kui sihtkontol on lubatud MFA ja parool arvati õigesti ära, ei kuvata kontot ohustatud kontona (teine autentimistegur pole täielik).

  - Paroolifail ei tohi olla suurem kui 10 MB. Kasutage ühte parooli rea kohta ja lisage loendis viimase parooli järele tühi rida (tagasijooksu).

- Olulised asjad, mida saate **teada oda andmepüügist, kinnitage** simulatsioonid.

  - Vaikimisi ei saa andmepüügilogimisserveri URL-i jaoks **kohandatud väärtust sisestada.**

  - Kui adressaat kasutab [](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) sõnumi andmepüügiks teatamiseks lisandmoodulit Luba aruandesõnumi lisandmoodul, ei pruugi te sõnumi kohta teatisi saada (kuna see on simuleeritud rünnak).

- Aruanded. Pärast simuleeritud rünnaku lõpule viimist saate aruande **koostamiseks** klõpsata nuppu Rünnaku üksikasjad.

- Üksikasjalikud juhised ja uued funktsioonid ründesimulaatoris leiate teemast [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).
