---
title: Pärand eDiscovery tööriistade pensionile jäämine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 262cca0feee17d1f929a5a94a4dd6c1ec317f6ec
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/21/2020
ms.locfileid: "43650564"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Pärand eDiscovery tööriistade pensionile jäämine

Uue ja täiustatud eDiscovery funktsiooni Microsoft 365 vastavuse Center tulemusena on järgmised pärand eDiscovery tööriistad ja commandlette lähikuudel pensionile:

- Kohapealse [eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) ja kohapealse [hoiab](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) Exchange ' i halduskeskus.

- Exchange Online PowerShelli cmdlet-käsud, mis toetavad kohapealse eDiscovery ja kohapealse hoiab. (Need cmdlet-käsud on ühiselt määratletud kui *-MailboxSearch cmdlet-käsud.) See hõlmab järgmisi cmdlet-käske:

    - [Uus MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Alusta-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stopp-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- [Otsing postkasti cmdlet-](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) käsu Exchange Online PowerShelli.
- Järgmised toimingud Exchange ' i veebiteenuste API-s:
    - [Getsearchablepostkastid](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [Setholdonpostkastid](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [Getholdonpostkastid](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Täpsem eDiscovery v 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Pensionile jäämise ajakava**:
- 1. aprill 2020: te ei saa luua uusi otsinguid ja hoiab, kuid saate endiselt käivitada, redigeerida ja kustutada olemasolevaid otsinguid omal vastutusel. Microsoft support ei toeta enam kohapealse eDiscovery & hoiab EAC.

- 1. juuli 2020: kohapealse eDiscovery & hoiab funktsiooni EAC paigutatakse kirjutuskaitstud režiimis. See tähendab, et teil on võimalik eemaldada ainult olemasolevad otsingud ja hoidmised.

**Lisateabe saamiseks vaadake**:

 - [Migreerimine pärand eDiscovery otsingud ja hoiab Microsoft 365 vastavuse keskus](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Pärand eDiscovery tööriistade pensionile jäämine](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [KKK kohapealse eDiscovery ja kohapealse valda kohta](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



