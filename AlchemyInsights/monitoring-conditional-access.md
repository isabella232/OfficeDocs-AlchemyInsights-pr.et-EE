---
title: Tingimusliku juurdepääsu jälgimine
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702899"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Exchange ' i tingimisi juurdepääsu jälgimine

Juurdepääsuõigusega kasutajatele antakse teatise meilisõnum, kui need ei vasta teie asutuse juurdepääsu nõuetele. Lahendamiseks soovitame teha ühte või mitut järgmistest lahendustest.
  
- Kui eeldatakse, et seade on registreeritud, Soovitage kasutajal minna ettevõtte portaali rakendusse ja veenduge, et see kuvatakse ettevõtte portaalis. Kui seda ei juhtu, peaks kasutaja seadme registreerima.
    
- Avage Azure ' i portaalis ** \> seadme nõuetele vastavuse häälestamine**. Klõpsake jaotises **kuvar** nuppu **seadme nõuetele vastavus**. Vaadake seadme nõuetele vastavuse aruandeid, et veenduda, kas kasutaja seade on märgitud nõuetele vastavaks. 
    
- Avage Azure ' i portaalis ** \> seadme nõuetele vastavuse häälestamine**. Klõpsake jaotises **haldamine**nuppu **poliitikad**. Veenduge, et nõuetele vastavuse poliitikate loendis oleks teie kasutaja seadmele määratud profiil. Kui profiili pole määratud, ei saa Intune kinnitada seadme nõuetele vastavuse olekut. 
    
- Kasutaja tingimusliku juurdepääsu määramise redigeerimine.
    
1. Azure ' i portaalis Avage ** \> tingimusjuurdepääsu \> poliitikate häälestamine**
    
2. Loendist poliitika valimine
    
3. Valige **kasutajad ja rühmad**
    
4. Kellegile teatud poliitika suunamiseks lisage need loendisse **kaasa** . Kui soovite tagada, et isik on poliitikast välja jäetud, lisage need loendisse **välista** . 
    
Lisateavet leiate [teemast tingimusliku juurdepääsu seadmete jälgimine](https://docs.microsoft.com/intune/conditional-access-exchange-monitor) .
  

