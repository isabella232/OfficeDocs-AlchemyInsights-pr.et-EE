---
title: Kaust 1336 RecoverableItems on täis
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
ms.openlocfilehash: 5c8d53ceabf2428f3d6d765040f1b789b6bbeda04a22dd7fde0d2d728fd17d93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061752"
---
# <a name="the-recoverable-items-folder-is-full"></a>Taastatavate üksuste kaust on täis

Postkastide Exchange Online on taastatavate üksuste kausta vaikesalvestuslimiit 30 GB. Taastatavate üksuste kausta salvestuslimiiti suurendatakse automaatselt 100 GB-ni, kui postkast on paigutatud ootele, e-juurdluse ootele või määratud säilituspoliitikale.

Kui kaust Taastatavad üksused jõuab salvestuslimiidini, mõjutab postkastifunktsioone järgmiselt.

- Kasutaja ei saa postkastist üksusi kustutada.

- Hallatava kausta abiline ei saa üksusi säilitussildi või hallatavate kaustasätete põhjal kustutada.

- Postkastide puhul, kus ühe üksuse taaste on lubatud või mis paigutatakse ootele, ei saa lehe kopeerimise kaitse protsess säilitada kasutaja redigeeritud üksuste versioone.

- Postkastide puhul, kus postkasti auditilogi on lubatud, ei saa kausta Taastatavad üksused alamkausta Auditid salvestada ühtegi postkasti auditilogi kirjet.

Postkastide korral, mis pole ootel, saavad `Search-Mailbox -SearchDumpsterOnly -DeleteContent` administraatorid powerShelli käsu Exchange Online kaustas Taastatavad üksused olevate üksuste kustutamiseks. Lisateavet vaadake järgmistest teemadest:

- [Sõnumite otsimine ja kustutamine](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Ootel olevate postkastide korral peavad administraatorid enne taastatavate üksuste kaustast üksuste kustutamist ootele jäetud üksuse eemaldama. Lisateavet leiate teemast Üksuste kustutamine ootel olevate pilvepõhiste [postkastide kaustas Taastatavad üksused.](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)

Kausta Taastatavad üksused täielikuks muutumise vältimiseks saavad administraatorid suurendada ootel olevate postkastide taastatavate üksuste kausta salvestuslimiiti ja häälestada postkasti säilituspoliitika, mis teisaldab üksused taastatavate üksuste kaustast kasutaja arhiivipostkasti. Vaadake [teemat Taastatavate üksuste kvoodi suurendamine ootel olevate postkastide jaoks.](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)
