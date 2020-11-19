---
title: Meilisõnumi tagasikutsumine või asendamine
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353502"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Meilisõnumi tagasikutsumine või asendamine rakenduses Microsoft 365

- Saate tagasi **kutsuda ainult teie asutuse inimestele saadetud sõnumeid**. Näiteks kui sõnum saadeti Gmaili aadressile, ei saa te seda meelde tuletada.
- Saate tagasi **kutsuda ainult Outlooki arvutist saadetud sõnumeid**. Kui kasutaja saadab Outlook for Maci või Outlooki veebirakenduse kaudu sõnumi, ei saa seda enam meelde tuletada.
- Rentniku administraatorina saate **kasutajate nimel sõnumeid tagasi kutsuda PowerShelli abil** (Lisateavet leiate teemast meilisõnumite [otsimine ja kustutamine](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).
- Administreerimiskeskuse sõnumeid ei saa tagasi kutsuda. Lisateavet leiate jaotisest "oma asutuse meilisõnumite otsimine ja kustutamine".

**Saadetud meilisõnumi tagasivõtmine või asendamine**

1. Valige Outlooki akna vasakus servas asuval paanil kaust saadetud üksused.
2. Avage sõnum, mille soovite tagasi kutsuda. Sõnumi avamiseks peate seda topeltklõpsama. Sõnumi valimine lugemispaanil kuvamisel ei luba teil sõnumit tagasi kutsuda.
3. Valige menüü Sõnum käsk **toimingud**, mida  >  **see sõnum tagasi kutsuda**.
4. Valige **Kustuta selle sõnumi lugemata eksemplarid** või **Kustuta lugemata eksemplarid ja asendage see uue sõnumiga**, seejärel valige **OK**.
5. Kui saadate asendus-sõnumi, koostage sõnum ja seejärel valige **saada**.
6. Sõnumi tagasivõtmise õnnestumine või ebaõnnestumine sõltub Outlooki adressaatide sätetest.

Lisateavet (sh tagasivõtmine) leiate teemast saadetud meilisõnumi [tagasikutsumine või asendamine](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

**_Oma asutuses meilisõnumite otsimiseks ja kustutamiseks_** on see lihtsaim viis, kui olete globaalne administraator. Kui te pole üldadministraator, peab teie konto olema lisatud e-juurdluse halduri rollirühma või vastavuse otsingu juhtimise rollile. Sõnumite kustutamiseks peate liituma organisatsiooni juhtimise rollirühma või otsingu ja likvideerimise rolliga. Nende rollide kasutusõigused määratakse [turbe & täitmise keskuses](https://protection.office.com/).

1. [Saate luua sisu otsimise](https://docs.microsoft.com/microsoft-365/compliance/content-search) , et leida sõnum, mille soovite kustutada.
2. [Looge ühendus turbe & vastavuse keskusega PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

Kui kasutate MFA-d (mitme teguriga autentimine), lugege teemat [ühenduse loomine Microsoft 365 turbe & nõuetele vastavuse keskus PowerShelli abil mitme teguriga autentimine](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).
