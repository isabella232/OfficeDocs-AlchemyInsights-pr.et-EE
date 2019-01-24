---
title: 1336 RecoverableItems kaust on täis
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: ee96abfa179c36ebaf43dbd327d4608b849395d3
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29466458"
---
# <a name="the-recoverable-items-folder-is-full"></a>Kausta Taastatavad üksused on täis

Office 365 Exchange Online'i postkasti kausta Taastatavad üksused vaikimisi mahupiirang on 30 GB. Kausta Taastatavad üksused mahupiirang on automaatselt suurendada 100 GB kui postkasti otsuse ootele, eDiscovery ootele, pannakse või osale Office 365 säilituspoliitika.
  
Kui kausta Taastatavad üksused jõuab salvestuslimiidi, mõjutatakse postkasti funktsionaalsust järgmiselt:
  
- Kasutaja ei saa kustutada postkastist üksusi.
    
- Hallatud kaustade abiline ei saa kustutada kaupu säilitussildi või hallatavasse kausta seaded.
    
- Postkastid, millel on lubatud ühe üksuse taastamine või ootele panna, ei saa kopeerimise kohta kirjutage lehe kaitse protsessi säilitada kasutaja muutis üksuste versioone.
    
- Postkastide on postkasti kontroll-logi sisse lülitatud, salvestatakse postkasti auditi logi kannete auditite alamkausta kaustas Taastatavad üksused.
    
Postkastide, mis ei ole registreeritud, saate kasutada administraatoritel on `Search-Mailbox -SearchDumpsterOnly -DeleteContent` käsu Exchange Online PowerShelli kustutada kausta Taastatavad üksused. Lisateabe saamiseks vaadake järgmisi teemasid: 
  
- [Otsida ja kustutada sõnumeid](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
Hoida postkastide administraatoritel on hold eemaldada, enne kui nad kustutatud üksuste kaustast Taastatavad üksused. Rohkem Lisateavet [taastatavate üksuste kausta kohta postkastidel hoidke üksuste kustutamine](https://docs.microsoft.com/en-us/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).
  
Aidata vältida liigset täielik kausta Taastatavad üksused, Administraatorid võivad suurendada taastatavate üksuste kaust postkastide hoida ja luua postkasti säilituspoliitika, mis teisaldab üksused kaustast Taastatavad üksused kasutaja arhiivi salvestuslimiidi postkasti. Vaata [Taastatavad üksused kvoot postkastide hoidke suurendada](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
  

