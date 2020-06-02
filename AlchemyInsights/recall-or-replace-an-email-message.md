---
title: E-kirja tagasivõtmine või asendamine
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: e958dab159e4dcc11f9c068bded3aa06ccd65c15
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509452"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Tagasivõtmine või asendamine e-kirja rakenduses Microsoft 365

- Te saate **ainult meenutada sõnumeid, mis saadetakse inimestele teie organisatsioonis**. Kui sõnum saadeti näiteks Gmaili aadressile, ei saa te seda meenutada.
- Saate **meenutada ainult sõnumeid, mis on saadetud Outlook 2016 arvuti jaoks**. Kui kasutaja saadab sõnumi, kasutades Outlook for Mac või Outlook veebis, ei mäleta seda.
- Kui olete administraator, võite **meenutada sõnumeid kasutajate nimel PowerShelli abil**. Administreerimiskeskusest ei saa sõnumeid meenutada. Lisateabe saamiseks Kerige allapoole "Otsi ja Kustuta e-kirju oma organisatsioonis".

**Saadetud meilisõnumi tagasivõtmine või asendamine**

1. Valige Outlooki aknast vasakul asuva kaustapaanil kaust saadetud.
2. Avage sõnum, mida soovite meelde tuletada. Sõnumi avamiseks peate topeltklõpsama. Sõnumi valimine lugemispaanil ei võimalda teil sõnumit meenutada.
3. Valige vahekaardil sõnum suvand **Tegevused**  >  **Meenuta seda sõnumit**.
4. Valige **kustutage selle sõnumi lugemata koopiad** või **kustutage lugemata koopiad ja asendage see uue sõnumiga**, seejärel valige **OK**.
5. Kui saadate asendussõnumi, koostage sõnum ja valige **saada**.
6. Sõnumi tagasikutsumise õnnestumine või nurjumine sõltub adressaatide sätetest Outlookis.

Lisateabe saamiseks, sealhulgas kuidas kontrollida tagasivõtmine, vaadake [tagasikutsumine või asendada e-kirja, mille te saatsite](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***E-kirjade otsimine ja kustutamine teie organisatsioonis*** Teie organisatsioonis meilisõnumite otsimiseks ja kustutamiseks on see lihtsaim, kui olete globaalne administraator. Kui te pole globaalne administraator, tuleb teie konto lisada eDiscovery halduri rollirühma või vastavuse otsingu haldamise rollile. Sõnumite kustutamiseks peate liituma organisatsiooni juhtimise rolligrupiga või otsingu ja Purge juhtimise rolliga. Nende rollide õigused on määratud [turvalisuse & vastavuse keskus](https://protection.office.com/).

1. [Saate luua sisuotsingu](https://docs.microsoft.com/microsoft-365/compliance/content-search) , et leida kustutatav sõnum.
2. [Ühendage Security & vastavuse keskus PowerShelli](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Kui kasutate MFA, vaadake [ühendust Microsoft 365 security & vastavuse Center PowerShelli mitme teguriga autentimine abil](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
