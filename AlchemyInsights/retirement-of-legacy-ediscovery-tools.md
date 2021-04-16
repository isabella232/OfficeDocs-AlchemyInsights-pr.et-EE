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
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798545"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Vanade e-juurdluse tööriistade kasutuselt kõrvaldamine

Microsoft 365 vastavuskeskuse uute ja täiustatud e-juurdluse funktsioonide tõttu lõpetatakse järgmiste kuude jooksul järgmised e-juurdluse tööriistad ja käsud.

- [Exchange'i halduskeskuses on](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [olemas e-juurdlus](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) ja kohtne ootel.

- Exchange Online'i PowerShelli cmdlet-käsud, mis In-Place e-juurdlust ja In-Place holds. (Need cmdlet-käsud tuvastatakse ühiselt kui *-MailboxSearchi cmdlet-käsud.) See hõlmab järgmisi cmdlet-käske.

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Exchange Online'i PowerShelli [cmdlet-käsk Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) (Otsingupostkast).
- Exchange'i veebiteenuste API-s on järgmised toimingud.
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Täpsem e-juurdlus v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Pensionile jäämise ajaskaala:**
- **1. juuli 2020** Te ei saa enam uusi otsinguid ja ootel otsimine, kuid saate olemasolevaid otsinguid ise käivitada, redigeerida ja kustutada. Microsofti tugiteenused ei toeta enam In-Place e-juurdluse & EAC-s ootel.
    
- **1. oktoobril 2020** In-Place E-juurdluse & EAC-s on ootel funktsioonid kirjutuskaitstud, nii et saate eemaldada ainult olemasolevad otsingud ja ootele pandud otsingud.

**Lisateavet leiate teemast**

 - [E-juurdluse pärandotsingute ja -salvestatud üksuste migreerimine Microsoft 365 vastavuskeskusesse](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Vanade e-juurdluse tööriistade kasutuselt kõrvaldamine](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [KKK e-juurdluse In-Place ja In-Place kohta](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



