---
title: Ühiskasutus väliskasutajatega ei tööta
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 02d79c1b1e112eb41e8c60ffa2ef28e429f76ada
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58304365"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Väliste kasutajate SharePoint sisu jagamisega seotud probleemide lahendamine

Veenduge, et väline ühiskasutus oleks teie asutuse jaoks sisse lülitatud.
  
1. Avage lehe [Teenused &amp; lisandmoodulid](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)lehel Microsoft 365 halduskeskus ja klõpsake nuppu **Saidid**.
    
2. Veenduge, et säte oleks "Sees". Kui valitud on "Ainult olemasolevad väliskasutajad", veenduge, et väline kasutaja on loendis Microsoft 365 halduskeskus.
    
Veenduge, et väline ühiskasutus oleks saidi jaoks sisse lülitatud. Klassikalise saidikogumi jaoks:
  
1. Klõpsake uues SharePoint vasakpoolsel paanil nuppu **Saidid**.
    
2. Valige sait või saidid ja klõpsake lindil nuppu **Ühiskasutus**.
    
Meeskonnatöö saidi puhul, mis kuulub Microsoft 365 rühma või suhtlussaidile:
  
- Nendel uutel saiditüüpidel on sama ühiskasutussäte, mis teie asutusel, välja arvatud juhul, kui kogu asutuse säte lubab failide ühiskasutust linkide abil, mis ei nõua sisselogimist. Sel juhul võimaldavad saidid ühiskasutust uute ja olemasolevate väliste kasutajatega, kes sisse logivad. Kindlate saitide sätte muutmiseks kasutage uut halduskeskust SharePoint PowerShelli. [Lisateave](https://go.microsoft.com/fwlink/?linkid=871863).
    
**Märkus.** Mis tahes saidi väline ühiskasutussäte võib olla piiravam kui teie asutuse kogu säte, kuid mitte rohkem läbivaatlik kui ettevõttes. 
  

