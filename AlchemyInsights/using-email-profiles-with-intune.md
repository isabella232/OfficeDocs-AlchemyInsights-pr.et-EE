---
title: E-posti profiilide kasutamine Intune ' i abil
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554978"
---
# <a name="using-email-profiles-with-intune"></a>E-posti profiilide kasutamine Intune ' i abil

Intune ' i abil saab luua ja juurutada mitmekeelseid meilikontosid (sisseehitatud) meiliklient mitme seadme platvormidel.

Lisateavet e-posti profiilidega seotud piirangute kohta (sh olemasolevate profiilide olemasolu ja selle kohta, kuidas eemaldada e-posti profiilid) leiate teemast [meilikontode lisamine seadmetele, mis kasutavad Intune](https://docs.microsoft.com/intune/email-settings-configure)' i.

Lisateavet iga seadme platvormi jaoks meiliprofiili loomise kohta leiate järgmistest teemadest.

[Androidi seadme sätted meili, autentimise ja sünkroonimise häälestamiseks Intune ' is](https://docs.microsoft.com/intune/email-settings-android)  
[IOS-i ja iPadOS seadmete meilikontode lisamine Microsoft Intune ' is](https://docs.microsoft.com/intune/email-settings-ios)  
[Microsoft Intune ' i meilikonto sätted Windows Phone ' i 8,1 seadmete jaoks](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Microsoft Intune ' is Windows 10 kasutavatele seadmetele mõeldud meilikontode meilisätted](https://docs.microsoft.com/intune/email-settings-windows-10)

**Levinud sünkroonimise probleem**

**Rakenduse KNOX Androidi meilikontos takistab kasutajate kontakte, kalendrit ja tööülesandeid, mida sünkroonitakse kasutaja seadmetega.**

KNOX Android KNOXi meilikonto profiilis annab administraatorile võimaluse otsustada, milliseid sisutüüpe sünkroonitakse seadmesse, seades need lubatud.

Kui mis tahes sisutüübi säte on seatud **pole konfigureeritud** (vaikesäte), ei sünkroonita seda sisutüüpi automaatselt. Kasutaja võib lubada sisutüübi, mida nad soovivad otse seadmele käsitsi lisada, kuid see konfiguratsioon kirjutatakse üle Intune ' i Poliitikasätte ja selle sisutüübi sünkroonimine peatub.

