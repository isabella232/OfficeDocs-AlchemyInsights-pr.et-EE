---
title: VPN-iga seotud probleemid
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
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554970"
---
# <a name="vpn-related-issues"></a>VPN-iga seotud probleemid

Virtuaalse privaatvõrgu ühenduvuse edukas rakendamine MDM-klientidele sõltub juurutatud profiilist, mis vastab õigesti VPN-i infrastruktuuri nõuetele. Teie uurimisel kasutatavate klientarvutite jaoks sobivate sätete leiate järgmistest teemadest. 

[Windows 10 ja Windowsi holograafiline seadme sätted Intune ' i abil VPN-ühenduste lisamiseks](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[VPN-i sätete lisamine iOS-i ja iPadOS seadmetes Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Androidi seadme sätted VPN-i konfigureerimiseks Intune-is](https://docs.microsoft.com/intune/vpn-settings-android)  
[VPN-i sätete lisamine opsüsteemis Microsoft Intune (macOS) seadmetes](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

Kui teie VPN-i profiil kasutab serdil põhinevat autentimist, veenduge, et VPN-profiiliga lingitud serdi ja kliendi autentimise serdi profiilid on edukalt juurutatud.

**Levinud probleemid**

**Juurutasin seadmesse VPN-I profiili. Intune näitab, et see oli edukas, kuid seade ei ühendu VPN-iga.**

Edukas olek tähendab seda, et Intune on profiili edukalt juurutanud konfigureeritud kujul. Kuid need konfiguratsioonid ei pruugi teie võrgu ja/või autentimise nõuetele vastavaks osutuda. Logige sisse infrastruktuuri ja autentimise teenuse (VPN server ja NPS/RADIUS serveri) kohta lisateabe saamiseks proovitud ühendust. Logide kogumiseks ja läbivaatamiseks peate võib-olla töötama võrgu infrastruktuuri meeskonnaga või kolmanda osapoole VPN-i tarnijaga.

**Kui Konfigureerin kohandatud VPN-I iOS-I jaoks, pole rakenduse VPN-i funktsioon saadaval.**

Rakenduse VPN iOS-i seadmetes Intune ' is on praegu saadaval kindlas teenusepakkujate ja partnerite loendis, kes peavad enne rakenduse VPN-i konfigureerimist täitma ka serdi eeltingimused. Lisateavet leiate teemast [rakenduse virtuaalse privaatvõrgu (VPN) häälestamine iOS-i/iPadOS seadmete jaoks Intune ' is](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

Lisateavet kõigi VPN-ühenduse tüüpide kohta Intune ' is leiate artiklist VPN- [profiilide loomine Intune ' i VPN-serveritega ühenduse](https://docs.microsoft.com/intune/vpn-settings-configure)loomiseks.  

**iOS on-demand VPN ei käivitu, kui konfigureeritud domeen on juurdepääsetav**

Automaatse VPN-i sätete testimiseks seadke järgmised väärtused.

Soovin teha järgmist. **hinnake iga ühenduste katset** 

Valige, kas soovite ühenduse luua: **vajadusel ühenduse loomine**

Kui kasutajad pääsevad juurde järgmistele domeenidele: **Target** *Domain Name*

Kui ülaltoodud konfiguratsioon pole edukas, lisage järgmine element.

Kui see URL pole kättesaadav, võtke ühendust VPN-iga: **BADURL**