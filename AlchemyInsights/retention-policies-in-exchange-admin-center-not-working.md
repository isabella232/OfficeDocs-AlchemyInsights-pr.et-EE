---
title: Säilituspoliitikad Exchange ' i halduskeskus ei tööta
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 3040365b9d686bcbcce60977ee9bdbbaffc70b24
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502603"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Säilituspoliitikad Exchange ' i halduskeskus

 **Probleem:** Äsja loodud või värskendatud Säilituspoliitikad Exchange ' i halduskeskus ei kohaldata postkastid või üksused on teisaldatud arhiivi postkasti või kustutatud. 
  
 **Algpõhjuste:**
  
- Põhjuseks võib olla see, et **hallatud Kaustaabimeest** pole kasutaja postkasti töödeldud. Hallatud kaustade abimees proovib töödelda iga postkasti oma pilvepõhise organisatsiooni kord iga seitsme päeva järel. Kui muudate säilitusmärgendit või rakendada mõnda muud säilituspoliitika postkasti, saate oodata, kuni hallatav kaust aitab töötleb postkasti või käivitage cmdleti Start-ManagedFolderAssistant käivitada hallatav kaust abimehe töödelda konkreetse postkasti. Selle cmdlet-käsu käitamine on kasulik säilituspoliitika või säilitusmärgendi sätete testimiseks või tõrkeotsinguks. Lisateabe saamiseks külastage [hallatava kausta abimehe käivitamine](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Lahendus:** Käivitage järgmine käsk käivitada hallatav kaust Assistant konkreetse postkasti:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- See võib ilmneda ka siis, kui **Retentionhold** on **lubatud** postkasti. Kui postkast on paigutatud RetentionHold, säilituspoliitika postkasti ei töödelda selle aja jooksul. Rohkem teavet kohta retentionhold säte vt: [postkasti säilitamise hoidke](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Lahendus:**
    
  - Kontrollige oleku RetentionHold kindla postkasti [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Käivitage järgmine käsk **keelata** retentionhold konkreetse postkasti:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Nüüd käivitage hallatav kausta abimees uuesti:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Märkus:** Kui postkast on väiksem kui 10 MB, hallatav kaust Assistant ei töötle automaatselt postkasti.
 
Exchange ' i halduskeskus säilituspoliitika kohta lisateabe saamiseks vaadake:
- [Säilitussildid ja Säilituspoliitikad](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Säilituspoliitika rakendamine postkastidele](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Säilitussiltide lisamine või eemaldamine](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Kuidas tuvastada tüüpi hoidke postkasti](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
