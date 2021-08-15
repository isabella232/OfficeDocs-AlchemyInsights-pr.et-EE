---
title: Meilisõnumi tagasivõtmine või asendamine
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
ms.openlocfilehash: 45882b49c5c47b3e0e4519e2339e6c68110bc75aebeaeac2d0ccd009bdfa3f7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024382"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Meilisõnumi tagasivõtmine või asendamine Microsoft 365

- Saate tagasi **võtta ainult sõnumeid, mis saadetakse teie ettevõtte inimestele.** Näiteks kui sõnum saadeti Gmaili aadressile, ei saa te seda tagasi kutsuda.
- Saate tagasi **võtta ainult arvuti Outlook saadetud sõnumeid.** Kui kasutaja saadab sõnumi, kasutades Outlook for Mac Outlooki veebirakendus, ei saa te seda tagasi kutsuda.
- Rentnikuadministraatorina saate **PowerShelli** abil kasutajate nimel sõnumeid tagasi võtta (lisateavet leiate teemast Meilisõnumite otsimine [ja kustutamine).](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)
- Halduskeskuses ei saa sõnumeid tagasi võtta. Lisateabe saamiseks liikuge kerides allapoole sõnani "Otsige ja kustutage meilisõnumeid oma asutuses".

**Saadetud meilisõnumi tagasivõtmine või asendamine**

1. Valige kaustapaanil akna Outlook kaust Saadetud.
2. Avage sõnum, mille soovite tagasi kutsuda. Sõnumi avamiseks peate seda topeltklõpsama. Sõnumi valimine lugemispaanil kuvamiseks ei võimalda teil sõnumit tagasi kutsuda.
3. Valige vahekaardil Sõnum nupp **Toimingud** Tuleta see sõnum  >  **tagasi**.
4. Valige **Kustuta selle sõnumi lugemata koopiad** või Kustuta **lugemata eksemplarid ja asendage see uue sõnumiga** ja seejärel valige **OK**.
5. Kui saadate asendussõnumi, koostage sõnum ja valige **Saada**.
6. Sõnumi tagasivõtmise õnnestumine või nurjumine sõltub adressaatide sätetest Outlook.

Lisateavet (sh tagasivõtmise kontrolli kohta) leiate teemast [Saadetud meilisõnumi tagasivõtmine või asendamine.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

***Ettevõttes meilisõnumite otsimiseks ja kustutamiseks*** on kõige lihtsam, kui olete üldadministraator. Kui te pole üldadministraator, tuleb teie konto lisada e-juurdluse halduri rollirühma või vastavusotsingu haldusrolli. Sõnumite kustutamiseks peate liituma organisatsioonihalduse rollirühma või otsingu- ja puhastushalduse rolliga. Nende rollide õigused määratakse turbe- [& vastavuskeskuses.](https://protection.office.com/)

1. [Kustutava sõnumi](https://docs.microsoft.com/microsoft-365/compliance/content-search) otsimiseks looge sisuotsing.
2. [Ühendus security & Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

Kui kasutate MFA-d (mitmikautentimist), lugege teemat Ühendus Microsoft 365 Security [& PowerShelli kasutamine mitmikautentimise abil.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
