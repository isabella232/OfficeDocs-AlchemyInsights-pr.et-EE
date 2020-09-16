---
title: Legacy-e-juurdluse tööriistade kasutuselt kõrvaldamine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2315c4c651a83f0ecc78c0171f32aba13bc93f8c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727779"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Legacy-e-juurdluse tööriistade kasutuselt kõrvaldamine

Microsoft 365 nõuetele vastavuse keskuses uute ja täiustatud e-juurdluse funktsioonide tulemusena aeguvad järgnevatel kuudel järgmised pärand e-juurdluse e-juurdluse tööriistad ja Commandlets.

- Kohapealne e [-juurdlus](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [ja kohapeal on Exchange](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) ' i halduskeskus.

- Exchange Online ' i PowerShelli cmdlet-käsud, mis toetavad kohapealset e-juurdlust ja kohapealset olemasolu. (Need cmdlet-käsud määratakse ühiselt *-MailboxSearch cmdlet-käskudeks.) See hõlmab järgmisi cmdlet-käske.

    - [Uus-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start – MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Exchange Online ' i PowerShelli cmdlet [-käsk Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) .
- Järgmised toimingud Exchange Web Services API-s:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Täiustatud e-juurdlus v 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Pensionile jäämise ajakava**:
- **1. juuli 2020** Uusi otsinguid ja ootelepaneku ei saa enam luua, kuid saate olemasolevaid otsinguid käivitada, redigeerida ja kustutada omal riisikol. Microsoft support ei toeta enam kohapealset e-juurdlust & kuulub EAC-sse.
    
- **1. oktoober 2020** Veebipõhine e-juurdlus & omab EAC-s funktsioone, mis kuvatakse kirjutuskaitstud režiimis, et saaksite eemaldada ainult olemasolevad otsingud ja ootelepanekud.

**Lisateavet leiate järgmistest teemadest**.

 - [Pärandist e-juurdluse otsingute migreerimine ja Microsoft 365 nõuetele vastavuse keskus](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Legacy-e-juurdluse tööriistade kasutuselt kõrvaldamine](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [KKK-kohapealne e-juurdlus ja kohapealne tööpõhimõte](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



