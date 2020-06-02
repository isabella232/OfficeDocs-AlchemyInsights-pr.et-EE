---
title: Outlooki töölaua tagasivõtmine või asendamine e-kirja
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: bb84363ae7d3c91750d5de789c091c7cebbbedc2
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502315"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Outlooki e-kirja tagasivõtmine või asendamine

- Nagu admin, saate **meenutada sõnumeid kasutajate nimel, kasutades PowerShelli**. Administreerimiskeskusest ei saa sõnumeid meenutada.
- Te saate **ainult meenutada sõnumeid, mis saadetakse inimestele teie organisatsioonis**. Kui sõnum saadeti näiteks Gmaili aadressile, ei saa te seda meenutada.
- Võite **meenutada ainult sõnumeid, mis on saadetud Outlook 2016 arvutist**. Kui kasutaja saadab sõnumi, kasutades Outlook for Mac või Outlook veebis, ei mäleta seda.

E-kirja tagasikutsumiseks või asendamiseks toimige järgmiselt.

1. Valige Outlooki aknast vasakul asuva kaustapaanil kaust saadetud.
1. Selle avamiseks topeltklõpsake sõnumit, mida soovite meenutada.
1. Valige vahekaart **sõnum** ja seejärel valige suvand **Tegevused**  >  **Meenuta seda sõnumit**.
1. Valige **kustutage selle sõnumi lugemata koopiad** või **kustutage lugemata koopiad ja asendage see uue sõnumiga**ning valige seejärel **OK**.
1. Kui saadate asendussõnumi, koostage sõnum ja valige siis **saada**.
1. Sõnumi tagasikutsumise õnnestumine või nurjumine sõltub adressaadi sätetest Outlookis. Juhised tagasivõtmist kontrollida, vt [käesoleva artikli](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Meilisõnumite otsimine ja kustutamine teie organisatsioonis

- Kui te pole globaalne administraator, tuleb teie konto lisada eDiscovery Manageri rollile või vastavuse otsingu haldamise rollile sõnumite otsimiseks. Sõnumite kustutamiseks peate liituma organisatsiooni juhtimise rolligrupiga või otsingu ja Purge juhtimise rolliga. Nende rollide õigused määratakse [turbe-ja Vastavuskeskuses](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Saate luua sisuotsingu](https://docs.microsoft.com/microsoft-365/compliance/content-search) , et leida kustutatav sõnum.
- [Ühendage turbe-ja Vastavuskeskus PowerShelli](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Kui kasutate mitme teguriga autentimine, vaadake [ühendust Microsoft 365 turvalisuse ja vastavuse Center PowerShelli mitme teguriga autentimine abil](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).