---
title: Tõrkeotsing probleemidele Ava Exploreris
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 49d6d449af6e718d70c9948a03f7e2e1e21517d2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323562"
---
# <a name="fix-problems-with-open-with-explorer"></a>Ava Exploreriga seotud probleemide lahendamine

Levinud probleemide lahendamine dokumenditeegi avamisel SharePoint OneDrive käsu **Ava Exploreriga** abil. 
  
- Kasutage Internet Explorer 10 või Internet Explorer 11. **Ava Exploreris** ei ühildu Microsoft Edge, Google Chrome'i, Firefoxi ega teistega. **Ava Exploreris** on keelatud kõigis brauserites peale Internet Exploreri. 
    
- **Exploreris avamine** pole tänapäevastes teekides SharePoint saadaval. Kasutage **selle asemel File Exploreris vaadet.** Valige **View options** View in File Explorer \> **(Kuva suvandid) File Exploreris**. Vaade File Exploreris ei ühildu Microsoft Edge, Google Chrome'i, Firefoxi ja teistega. **Vaade File Exploreris on** saadaval ainult Internet Exploreris. 
    
- Veenduge, et Teenus WebClient töötaks. Tippige Windows käivitamine, valige käsk Käivita töölauarakendus, tippige services.msc ja vajutage sisestusklahvi (Enter). Liikuge kerides allapoole teenuseni WebClient ja veenduge, et **veerus Olek** oleks kuvatud tekst "Töötab". Kui see nii ei ole, topeltklõpsake teenust, klõpsake nuppu **Start** ja seejärel nuppu **OK**. (Võimalik, et peate teenuse esmalt lubama, valides **väljal** Käivitustüüp kas Käsitsi  **või** Automaatne.) 
    
**Märkus.** Teegi avamine File Exploreris on mugav, kui teil on vaja kopeerida või teisaldada mitu faili ja kausta üks kord, kuid kui soovite teegis regulaarselt töötada, soovitame seda sünkroonida. File Exploreris avamisega seotud probleemide tõrkeotsinguks lugege [teemat Ava Exploreris.](https://go.microsoft.com/fwlink/?linkid=871665) Lisateavet sünkroonimise häälestamise kohta leiate teemast [SharePoint failide sünkroonimine uue OneDrive'i sünkroonimisrakendus klientrakendusega.](https://go.microsoft.com/fwlink/?linkid=871666)
  
Lisateavet leiate artiklist SharePoint Online'i probleemide tõrkeotsinguks käsu ["Ava](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) Exploreris" kasutamine. 
  

