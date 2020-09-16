---
title: E-posti profiilide kasutamine Intune ' i abil
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653284"
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

