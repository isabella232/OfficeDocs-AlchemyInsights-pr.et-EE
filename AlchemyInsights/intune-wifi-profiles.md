---
title: Wi-Fi-profiilide Intune
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555005"
---
# <a name="intune-wi-fi-profiles"></a>Wi-Fi-profiilide Intune

MDM-i klientide Wi-Fi-ühenduvuse edukas rakendamine sõltub õigesti juurutatud profiilist, mis vastab ettevõtte Wi-Fi infrastruktuuri nõuetele. Uuritud klientarvutite vastavate sätete läbivaatamiseks lugege järgmisi teemasid. 

[Wi-Fi-sätete lisamine Androidi kasutavatele seadmetele Microsoft Intune ' is](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Wi-Fi-sätete lisamine Android Enterprise ' i jaoks mõeldud ja täielikult hallatavatele seadmetele Microsoft Intune ' is](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Wi-Fi-sätete lisamine iOS-i ja iPadOS seadmete jaoks Microsoft Intune ' is](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Wi-Fi-sätete lisamine Windows 10 ja uuemate seadmete jaoks Intune ' is](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Windowsi seadmetes Wi-Fi-sätete importimine Intune ' is](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Levinud probleemid**

**Juurutan Wi-Fi-profiili, mis sõltub Wi-Fi-profiilis määratud kasutatavast serdist. Konfiguratsiooni profiilid kuvatakse siiski tõrke olek.**

Kontrollige, kas teie seade sai serdi kätte.

1. Tehke Intune ' is valik **kõik seadmed** ja valige seade > **seadme konfiguratsioon**.

2. Kontrollige, kas kõik oodatud profiilid on loendis ja edukas olekus.

3. Kui teie sertide tarneahelas on vaheserdid, siis veenduge, et Androidi profiilis oleks need juurutatud Androidi seadmetes.

    Serdi oleku kontrollimiseks valige **seadme konfiguratsiooni**  >  **profiilid**  >  **Android Kesktase ca**  >  **Atribuudid**  >  **usaldusväärsed serdid**.

Kui kuvatakse endiselt tõrked, vaadake jaotist protseduurid ja tõrkeotsing. Lisateavet leiate teemast [Microsoft Intune ' i SCEP serdi profiilide tõrkeotsingu ülevaade](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**Juurutasin seadmes Wi-Fi-profiili. Intune näitab, et see oli edukas, kuid seade ei Ühenda Wi-Fi-võrguga.**

Edukas olek tähendab seda, et Intune on profiili edukalt juurutanud konfigureeritud kujul. Kuid need konfiguratsioonid ei pruugi teie võrgu ja/või autentimise nõuetele vastavaks osutuda. Proovitud ühenduse kohta leiate lisateavet teemast logid sisse infrastruktuuri ja autentimise teenuses (Wi-Fi-pääsupunkti kontrolleri ja NPS/RADIUS serveri kaudu). Logide kogumiseks ja läbivaatamiseks peate võib-olla töötama võrgu infrastruktuuri meeskonnaga või muu tootja WiFi-tarnijaga.