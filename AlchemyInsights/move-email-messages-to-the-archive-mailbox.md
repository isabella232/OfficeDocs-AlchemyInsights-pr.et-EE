---
title: Liikumine e-kirju arhiivi postkasti
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 41d6825b568263fb7b09066b65235aa348415bae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28286123"
---
Arhiivi postkasti üksuste arhiivimise probleeme. Veenduge, et olete sooritanud järgmised sammud:
  
1. Kinnitada, et on **arhiivi postkasti** on aktiivne. Kui ei, siis kasutage [käesoleva artikli](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) juhiseid arhiivi postkasti lubamine. 
    
2. Exchange'i halduskeskuse abil, valige **Säilitussiltide** alusel **Nõuetele vastavuse tagamine**, **Teisalda arhiivi** meetmega, mis sisaldab soovitud **Säilituseani** **säilitussildi** loomine.
    
3. Exchange'i halduskeskuse abil, valige **Säilituspoliitikad**, **Säilituspoliitika** loomine ja **Teisalda arhiivi** säilitussildi lisamine poliitika. 
    
4. [Säilituspoliitika määrata](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) konkreetse kasutaja postkasti. Sedasama kohaldatakse ka **esmase** ja **arhiivipostkasti** . 
    
Kasutaja postkasti peaks nüüd olema kaupade liigutamiseks arhiivipostkasti arhiivipoliitika. Tuleb sundida õnnestus kausta abimehe (MFA) ja uued sätted rakenduvad kasutaja postkasti. Käivitada samal ajal [ühendatud EKSO PowerShelli](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) alustada abiline konkreetsele postkastile järgmine käsk: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Lisainfot arhiivipoliitika seadistamise kohta, vaadake teemat [arhiivi ja kustutamise poliitika postkastide](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

