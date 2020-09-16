---
title: Kliendi autentimise serdi juurutamise tõrkeotsing
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
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658982"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Kliendi autentimise serdi juurutamise tõrkeotsing

Intune ' i NDES/SCEP ja PKCS/PFX-i kliendi sertide profiile kasutatakse tavaliselt koos muude profiilidega (nt WiFi, VPN ja meiliaadress), et kasutajad saaksid autentida ettevõtte ressursse. Kui need profiili tüübid on lingitud kliendi serdi profiiliga, sõltub selle profiili edukas rakendamine.

Kliendi serdi profiili algse infrastruktuuri häälestus ja seotud konfiguratsioon nõuavad sageli tõrkeotsingut. Üksikasjalikud juhised NDES konnektori edukaks häälestamiseks ja tõrkeotsingu juhised serdi juurutusega seotud probleemide isoleerimiseks leiate järgmistest teemadest. 

- [Konfigureeri infrastruktuur, et toetada SCEP Intune ' i abil](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Microsoft Intune ' i SCEP serdi profiilide tõrkeotsingu ülevaade](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Kasutage konfiguratsiooni kinnitamiseks viidatud PowerShelli skripte. Lisateavet leiate artiklist [Intune ' i serdi konnektori kinnitamise skriptid](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Muud levinud probleemid**

**Kui proovin installida Intune ' i serdi konnektori NDES konnektori serverisse, kuvatakse teade "serdi taotluses olevat parooli ei saa kontrollida. Võimalik, et seda on juba kasutatud. Hankige selle päringuga esitamiseks uus parool. "**  

See sõnum tähendab, et peate käivitama serdi konnektori installi administraatorina.

Mõnes keskkonnas peavad Intune ' i serdiga serverid kasutama Intune ' iga ühenduse loomiseks puhverserverit ja seega peab serdi konnektor kasutama puhverserverit. Mõnel juhul ignoreerib NDES konnektor konfigureeritud puhverserveri sätteid ja võib olla vajalik puhverserveri sätete konfigureerimine LocalSystem turbe kontekstis. 
 
Lahenduseks on Internet Exploreri käivitamine SÜSTEEMIna ja puhverserveri konfigureerimine IE-s. Pärast Intune Connector Service ' i taaskäivitamist loob NDES konnektor Intune ' i.

**NDES ei saa kasutaja seadmeid enam SCEP sertidest.**

On võimalik, et NDES serverile väljastatud kliendi autentimine, mis on määratud NDES konnektori installimisel, on aegunud või on puudu. Lahendamiseks tehke järgmist. 
 
1. Desinstallige NDES konnektor.  
2. Kasutage järgmisi andmeid uue kliendi autentimise või serveri autentimise serdi taotlemiseks. 
 
    - Teema nimi: CN = väline FQDN  
    - Teema alternatiivne nimi (mõlemad on nõutavad): DNS = väline FQDN, DNS = sisemine FQDN 
 
3. Installige NDES konnektor uuesti uue serdiga.