---
title: 1336 RecoverableItems kausta on täis
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 4f0cba480fcc05114abd8f370b84e9a37e5f2804
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510748"
---
# <a name="the-recoverable-items-folder-is-full"></a>Kausta Taastatavad üksused on täis

Exchange Online ' i postkasti vaikimisi ladustamise piirang kausta Taastatavad üksused on 30 GB. Taastatav üksuste kausta talletuslimiit suurendatakse automaatselt 100 GB-ga, kui postkast pannakse kohtuprotsessi Hold, eDiscovery ootel või on määratud säilituspoliitika.

Kui Taastatavad üksused kausta jõuab ladustamise piirang, postkasti funktsionaalsust mõjutab järgmistel viisidel:

- Kasutaja ei saa kustutada üksusi postkasti.

- Hallatav Kaustaabimees ei saa kustutada üksusi, mis põhinevad säilitusmärgil või hallatud kaustasätel.

- Postkastid, mis on ühe üksuse taastamine lubatud või on paigutatud, Copy-on-kirjutada lehe kaitse protsess ei saa hallata kasutaja redigeeritud üksuste versioonid.

- Postkastid, mis on postkasti auditilogi logimise lubatud, ei saa salvestada postkasti audit Logi kirjeid kausta Taastatavad üksused audit alamkausta.

Postkastid, mis ei ole, administraatoritel saab kasutada `Search-Mailbox -SearchDumpsterOnly -DeleteContent` käsku Exchange Online PowerShelli üksuste kustutamiseks kausta Taastatavad üksused. Lisateavet vaadake järgmistest teemadest:

- [Sõnumite otsimine ja kustutamine](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Otsing-postkast](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Postkastid, mis on hoida, administraatoritel eemaldada hoidke enne, kui nad saavad kustutatud üksuste kaustast Taastatavad üksused. Lisateabe saamiseks vaadake [kustutage üksused pilvepõhiste postkastide kausta Taastatavad üksused hoida](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Et vältida Taastatavad üksused kausta saada täis, administraatoritel võib suurendada ladustamise piirang Taastatavad üksused kausta postkastid hoidke ja seadistada postkasti säilituspoliitika, mis teisaldab üksused kausta Taastatavad üksused kasutaja arhiivi postkasti. Vaadake [suurendada Taastatavad üksused kvoodi postkasti hoida](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
