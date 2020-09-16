---
title: 1336 RecoverableItems kaust on täis
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741263"
---
# <a name="the-recoverable-items-folder-is-full"></a>Kaust Taastatavad üksused on täis

Exchange Online ' i postkastide jaoks on kausta Taastatavad üksused vaikeväärtuseks 30 GB. Kausta Taastatavad üksused salvestusruumi limiiti suurendatakse automaatselt 100 GB-ni, kui postkast paigutatakse ootele, e-juurdluse ootele või määratakse säilituspoliitika.

Kui kaust Taastatavad üksused jõuab salvestusruumi piirmäärani, mõjutab see postkasti funktsioone järgmiselt.

- Kasutaja ei saa postkastist üksusi kustutada.

- Hallatava kausta assistent ei saa üksusi säilitus-või hallatava kausta sätete põhjal kustutada.

- Kui postkastid, millel on ühe üksuse taastamine lubatud või on paigutatud ootele, ei saa koopiat kirjutamise lehel säilitada kasutaja poolt redigeeritud üksuste versioone.

- Postkastide korral, millel on lubatud postkast audit, ei saa Postkasti auditilogi kirjeid salvestada kausta Taastatavad üksused.

Kui postkastid pole ootel, saavad administraatorid kasutada `Search-Mailbox -SearchDumpsterOnly -DeleteContent` Exchange Online PowerShelli käsku, et kustutada üksused kaustas Taastatavad üksused. Lisateavet vaadake järgmistest teemadest:

- [Sõnumite otsimine ja kustutamine](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Otsing – postkast](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Postkastid, mis on ootel, peavad administraatorid eemaldama ootelepaneku, enne kui nad saavad üksused kaustast Taastatavad üksused kustutada. Lisateavet leiate teemast [pilvepõhise postkasti taastatavate üksuste kaustas olevate üksuste kustutamine ootel](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Kui soovite, et kausta Taastatavad üksused ei muutuks täielikuks, võivad administraatorid ootel olevate postkastide kausta taastatavate üksuste salvestusruumi suurendada ja häälestada postkasti säilituspoliitika, mis teisaldab üksused kaustast Taastatavad üksused kasutaja arhiivi postkasti. Vaadake teemat [postkasti taastatavate üksuste kvoodi suurendamine ootele](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
