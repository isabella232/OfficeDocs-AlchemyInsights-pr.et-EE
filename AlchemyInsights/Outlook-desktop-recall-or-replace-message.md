---
title: Outlooki töölaua tagasikutsumine või asendamine e-kirja
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: aced684777ef82860b969aea8825699b78b04c5a
ms.sourcegitcommit: aad9f863bc9fd7d5522c480bd1a7d15f3a80ff4f
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/15/2019
ms.locfileid: "30657040"
---
# <a name="recall-or-replace-an-email-message"></a>Tagasi kutsuda või asendada e-kirja

- Admin, võite **meenutavad sõnumid PowerShelli abil kasutajate nimel**. Ei mäleta sõnumeid halduskeskuse kaudu.
- Saab **ainult turult sõnumid, mis saadetakse ettevõtte**. Kui sõnum saadeti Gmaili aadressi, näiteks ei mäleta seda.
- Saab **ainult turult kirjad Outlook 2016 PC**. Kui kasutaja saadab sõnumi, kasutades Outlook for Mac või Outlook veebis, ei mäleta seda.

Tagasikutsumise või asendamise e-kirja:

1. Valige Outlooki vasakul paanil kausta kausta Saadetud.
1. Topeltklõpsake selle avamiseks tagasi kutsutava.
1. Valige **sõnum** jaotises ja seejärel valige **toiminguid** > **Kutsu see sõnum tagasi**.
1. Valige **kustutada selle sõnumi lugemata eksemplarid** või **kustutada lugemata eksemplarid ja asendada need uue sõnumiga**ja seejärel klõpsake **nuppu OK**.
1. Asendamine sõnumi saatmisel Koosta sõnum ja valige **saada**.
1. Sõnumi tagasikutsumise takistavaid sõltub teenuse kasutaja Outlooki sätteid. Kontrollida tόhistamise kohta leiate [käesoleva artikli](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Otsida ja kustutada e-kirju teie organisatsiooni

- Kui sa ei ole globaalne admin, lisatakse teie konto e-juurdluse haldur rolli või vastavuse Otsi rollirühma otsida sõnumeid. Sõnumite kustutamiseks peate organisatsioonihalduse rollirühma või otsingu- ja Likvideeri RBAC-roll. Nende rollide õiguste määratakse [Turve ja vastavus center](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Loo sisu otsida](https://docs.microsoft.com/office365/securitycompliance/content-search) leida sõnumi kustutamiseks.
- [Turvalisus ja vastavus Center PowerShelli](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Mitmekordne autentimine kasutamisel vaadake [ühenduse loomine Office 365 turvalisuse ja nõuetele vastavuse Center PowerShelli kasutamine mitmefaktorilist autentimist](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).