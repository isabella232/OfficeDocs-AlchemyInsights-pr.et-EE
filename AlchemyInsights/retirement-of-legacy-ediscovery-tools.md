---
title: Vanade e-juurdluse tööriistade kasutuselt kõrvaldamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2e7f898ac1a9e9469f633192be18e2a3a362023c83c9e510593196b5a4a0daf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074649"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Vanade e-juurdluse tööriistade kasutuselt kõrvaldamine

Uute ja täiustatud e-juurdluse funktsioonide tõttu Microsoft 365 järgmised e-juurdluse tööriistad ja käsud järgmistel kuudel.

- [E-juurdluse ja](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [kohakohane omab](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) Exchange halduskeskuses.

- PowerShelli Exchange Online cmdlet-käsud, mis In-Place e-juurdlust ja In-Place holds. (Need cmdlet-käsud tuvastatakse ühiselt kui *-MailboxSearchi cmdlet-käsud.) See hõlmab järgmisi cmdlet-käske.

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- [PowerShelli otsingupostkasti cmdlet-Exchange Online.](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps)
- Järgmised toimingud Exchange Web Services API-s.
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Pensionile jäämise ajaskaala:**
- **1. juuli 2020** Te ei saa enam uusi otsinguid ja ootel otsimine, kuid saate olemasolevaid otsinguid ise käivitada, redigeerida ja kustutada. Microsofti tugiteenused ei toeta enam In-Place e-juurdluse & EAC-s ootel.
    
- **1. oktoobril 2020** In-Place E-juurdluse & EAC-s on ootel funktsioonid kirjutuskaitstud, nii et saate eemaldada ainult olemasolevad otsingud ja ootele pandud otsingud.

**Lisateavet leiate teemast**

 - [E-juurdluse pärandotsingute migreerimine ja nende Microsoft 365 vastavuskeskus](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Vanade e-juurdluse tööriistade kasutuselt kõrvaldamine](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [KKK e-juurdluse In-Place ja In-Place kohta](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



