---
title: Outlook Meilisõnumi tagasivõtmine või asendamine töölaual
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 33fe7ebd53d7ff11dbab54ce589aaf58e68c633be4d83a3cdfb00edc7752430e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918391"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Meilisõnumi tagasivõtmine Outlook asendamine

- Administraatorina saate **PowerShelli abil kasutajate nimel sõnumeid tagasi võtta.** Halduskeskuses ei saa sõnumeid tagasi võtta.
- Saate tagasi **võtta ainult sõnumeid, mis saadetakse teie ettevõtte inimestele.** Kui sõnum saadeti näiteks Gmaili aadressile, ei saa te seda tagasi kutsuda.
- Saate tagasi **võtta ainult arvutist Outlook 2016 saadetud sõnumeid.** Kui kasutaja saadab sõnumi, kasutades Outlook for Mac Outlooki veebirakendus, ei saa te seda tagasi kutsuda.

Meilisõnumi tagasikutsumiseks või asendamiseks:

1. Valige kaustaaknast vasakul oleval kaustapaanil Outlook kaust Saadetud üksused.
1. Selle avamiseks topeltklõpsake sõnumit, mille soovite tagasi kutsuda.
1. Valige menüü **Sõnum** ja seejärel valige Toimingud **Tuleta** see sõnum  >  **tagasi.**
1. Valige **Kustuta selle sõnumi lugemata koopiad** või Kustuta **lugemata eksemplarid** ja asendage see uue sõnumiga ja seejärel valige **OK**.
1. Kui saadate asendussõnumi, koostage sõnum ja seejärel valige **Saada**.
1. Sõnumi tagasivõtmise õnnestumine või nurjumine sõltub adressaadi sätetest Outlook. Tagasivõtmise kontrolli juhised leiate sellest [artiklist.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

Ettevõttes meilisõnumite otsimine ja kustutamine

- Kui te pole üldadministraator, tuleb sõnumite otsimiseks lisada oma konto e-juurdluse halduri rolli või nõuetele vastavuse otsingu haldamise rolli. Sõnumite kustutamiseks peate liituma organisatsioonihalduse rollirühma või otsingu- ja puhastushalduse rolliga. Nende rollide õigused määratakse turbe- [ja vastavuskeskuses.](https://go.microsoft.com/fwlink/?linkid=2083731)
- [Kustutava sõnumi](https://docs.microsoft.com/microsoft-365/compliance/content-search) otsimiseks looge sisuotsing.
- [Ühendus turbe- ja vastavuskeskuse PowerShelli.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)

Kui kasutate mitme teguriga autentimist, lugege Ühendus Microsoft 365 ja [vastavuskeskuse PowerShelli kasutamist mitme teguriga autentimise abil.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)