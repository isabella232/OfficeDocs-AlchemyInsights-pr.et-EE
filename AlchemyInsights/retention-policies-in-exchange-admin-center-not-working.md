---
title: Exchange ' i administreerimiskeskuse poliitikate säilitamine ei tööta
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
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740506"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Säilituspoliitika Exchange ' i administreerimiskeskuses

Kui soovite, et me käivitaks allpool mainitud sätete automatiseeritud kontrolli, valige nupp tagasi <--selle lehe ülaosas ja seejärel sisestage selle kasutaja meiliaadress, kellel on säilituspoliitika probleeme.

 **Probleem:** Exchange ' i administreerimiskeskuse äsja loodud või värskendatud säilituspoliitika ei rakendu postkastidele ega üksustele ei teisaldata arhiivi postkasti ega kustutatud. 
  
 **Juure põhjused.**
  
- Selle põhjuseks võib olla, et **hallatud kaustade abiline** pole kasutaja postkasti töödelnud. Hallatud kaustade assistent proovib töödelda iga teie pilvepõhise asutuse postkasti iga seitsme päeva järel. Kui muudate säilituse silti või rakendate postkastile mõne muu säilituspoliitika, võite oodata, kuni hallatav kaust teie postkasti töötleb, või käivitage ManagedFolderAssistant cmdlet-käsk, et käivitada hallatavate kaustade abiline kindla postkasti töötlemiseks. Selle cmdlet-käsu käivitamine on kasulik säilituspoliitika või säilituse siltide sätete katsetamiseks või tõrkeotsinguks. Lisateavet leiate teemast [hallatava kausta abilise käivitamine](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Lahendus:** Hallatava kausta abilise käivitamiseks kindla postkasti korral käivitage järgmine käsk.
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- See võib ilmneda ka juhul, kui postkastis on **RetentionHold** **lubatud** . Kui postkast on paigutatud RetentionHold, siis postkasti säilituspoliitika ei töödelda selle aja jooksul. RetentionHold Informaton kohta leiate lisateavet järgmistest teemadest: [postkasti säilituse ootelepanek](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Lahendus**
    
  - Kontrollige, kas RetentionHold säte on kindlas postkastis, mis asub [ekso PowerShellis](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps).
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - RetentionHold **keelamiseks** kindlal postkastil käivitage järgmine käsk.
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Käivitage uuesti hallatavate kaustade abiline.
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Märkus:** Kui postkast on väiksem kui 10 MB, siis ei töötle hallatud kaustade assistent postkasti automaatselt.
 
Lisateavet Exchange ' i administreerimiskeskuse poliitikate kohta leiate järgmistest teemadest.
- [Säilituse siltide ja säilituspoliitika põhimõtted](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Säilituspoliitika rakendamine postkastidele](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Säilituse siltide lisamine või eemaldamine](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Postkastile paigutatud ootelepaneku tüübi tuvastamine](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
