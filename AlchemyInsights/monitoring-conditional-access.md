---
title: Tingimusjuurdepääsu jälgimine
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713714"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Exchange ' i tingimusjuurdepääsu jälgimine

Tingimusjuurdepääsu sihtkasutajad saavad meilimeili, kui need ei vasta teie organisatsiooni juurdepääsunõuetele. Probleemi lahendamiseks soovitame ühte või mitut järgmistest lahendustest:
  
- Kui eeldatakse, et seade on registreeritud, soovitame kasutajal minna ettevõtteportaali rakendusse ja veenduda, et see kuvatakse ettevõtteportaalis. Kui ei ole, kasutaja peaks registreeruda seade.
    
- Azure ' i portaal minna **Intune \> seadme nõuetele**. Klõpsake **Monitor** jaotises monitor **seadme vastavus**. Vaadake seadme vastavusaruannet veendumaks, et kasutaja seade on märgitud vastavaks. 
    
- Azure ' i portaal minna **Intune \> seadme nõuetele**. Klõpsake jaotises **Halda** **poliitikad**. Vastavuse poliitika loendis veenduge, et profiil on määratud teie kasutaja seadmesse. Kui ühtegi profiili pole määratud, ei saa Intune kinnitada seadme vastavusolekut. 
    
- Redigeerige kasutaja tingimusjuurdepääsu määramist.
    
1. Azure ' i portaal minna **Intune \> tingimusjuurdepääsu \> poliitikad**
    
2. Valige loendist soovitud poliitika
    
3. Klõpsake valikul **kasutajad ja rühmad**
    
4. Teatud poliitika kellelegi sihtimiseks lisage need **kaasamisloendisse** . Et tagada, et inimene on poliitikast välja jäetud, lisage need **välisnimekirja** . 
    
Loe lähemalt: [Kuidas jälgida tingimusjuurdepääsu seadmed](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

