---
title: Meiliprofiilide kasutamine Intune'iga
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
ms.openlocfilehash: b1653b73e7296e7eed411ae73c19342a1187b2eb7e287cff4339ea0ca32d75c1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919419"
---
# <a name="using-email-profiles-with-intune"></a>Meiliprofiilide kasutamine Intune'iga

Intune'i saab kasutada meiliprofiilide loomiseks ja juurutamiseks kohaliku (sisseehitatud) meilikliendi jaoks mitmel seadmeplatvormil.

Teavet meiliprofiilidega seotud piirangute (sh olemasolevate profiilide kasutamise ja meiliprofiilide eemaldamise kohta) kohta leiate teemast Meilisätete lisamine [Intune'i abil seadmetesse.](https://docs.microsoft.com/intune/email-settings-configure)

Lisateavet iga seadmeplatvormi jaoks meiliprofiilide loomise kohta leiate teemast

[Androidi seadme sätted meili, autentimise ja sünkroonimise konfigureerimiseks Intune'is](https://docs.microsoft.com/intune/email-settings-android)  
[Meilisätete lisamine iOS-i ja iPadOS-i seadmete jaoks Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Meiliprofiili sätted Microsoft Intune seadmetes, kus töötab Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Meiliprofiili sätted seadmetes, kus Windows 10 Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Levinud sünkroonimisprobleem**

**Androidi meiliprofiili KNOX takistab kasutaja kontakte, kalendrit ja ülesandeid sünkroonida kasutaja seadmetega.**

Android KNOX-i meiliprofiil KNOX pakub administraatorile võimalust otsustada, millised sisutüübid seadmega sünkroonitakse, määrates iga seadme jaoks lubatud.

Kui mõne sisutüübi sätteks on seatud **Pole konfigureeritud** (vaikesäte), siis seda sisutüüpi automaatselt ei sünkroonita. Kasutaja võib lubada soovitud sisutüübi otse seadmes käsitsi, kuid Intune'i poliitikasäte kirjutab selle konfiguratsiooni üle ja selle sisutüübi sünkroonimispeatused.

