---
title: Outlooki töölaua tagasivõtmine või asendamine meilisõnumiga
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
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663986"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Outlooki meilisõnumi tagasikutsumine või asendamine

- Administraatorina saate **sõnumeid tagasi kutsuda PowerShelli abil kasutajate nimel**. Administreerimiskeskuse sõnumeid ei saa tagasi kutsuda.
- Saate tagasi **kutsuda ainult teie asutuse inimestele saadetud sõnumeid**. Kui sõnum saadeti näiteks Gmaili aadressile, ei saa seda enam meelde tuletada.
- Saate tagasi **kutsuda ainult Outlook 2016 arvutist saadetud sõnumeid**. Kui kasutaja saadab Outlook for Maci või Outlooki veebirakenduse kaudu sõnumi, ei saa seda enam meelde tuletada.

Meilisõnumi tagasivõtmiseks või asendamiseks tehke järgmist.

1. Valige Outlooki akna vasakus servas asuval paanil kaust saadetud üksused.
1. Topeltklõpsake sõnumit, mille soovite selle avamiseks meelde jätta.
1. Valige vahekaart **sõnum** ja seejärel klõpsake nuppu **toimingud**, et  >  **see sõnum tagasi kutsuda**.
1. Valige **Kustuta selle sõnumi lugemata eksemplarid** või **Kustuta lugemata eksemplarid ja asendage see uue sõnumiga**ning seejärel valige **OK**.
1. Kui saadate asendus-sõnumi, koostage sõnum ja seejärel valige **saada**.
1. Sõnumi tagasivõtmise õnnestumine või ebaõnnestumine sõltub Outlooki adressaadi sätetest. Lisateavet tagasivõtmise kontrollimise kohta leiate [sellest artiklist](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Oma asutuse meilisõnumite otsimine ja kustutamine

- Kui te pole üldadministraator, tuleb teie konto lisada sõnumite otsimiseks e-juurdluse halduri rollile või vastavuse otsingu juhtimise rollile. Sõnumite kustutamiseks peate liituma organisatsiooni juhtimise rollirühma või otsingu ja likvideerimise rolliga. Nende rollide load määratakse [turbe-ja vastavuskontrolli keskuses](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Saate luua sisu otsimise](https://docs.microsoft.com/microsoft-365/compliance/content-search) , et leida sõnum, mille soovite kustutada.
- [Looge ühendus turbe-ja vastavuskontrolli keskusega PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Kui kasutate mitme teguri autentimist, lugege teemat [ühenduse loomine Microsoft 365 turbe ja ühilduvuse keskusega PowerShell, kasutades mitut tegurit autentimine](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).