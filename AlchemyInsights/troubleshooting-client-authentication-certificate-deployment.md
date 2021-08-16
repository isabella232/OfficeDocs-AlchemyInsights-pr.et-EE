---
title: Kliendiautentimise serdi juurutamise tõrkeotsing
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
ms.openlocfilehash: 78520b416a72a3c93a3d2e7726948d59f83e681d4f09078c2a3cefac7bf1db3d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020800"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Kliendiautentimise serdi juurutamise tõrkeotsing

Intune'i NDES-i/SCEP-i ja PKCS-i/PFX-i kliendisertide profiile kasutatakse tavaliselt koos muude profiilitüüpidega (nt Wifi, VPN ja meil), et võimaldada kasutajatel ettevõtte ressurssidega autentida. Kui need profiilitüübid on lingitud kliendi sertimisprofiiliga, sõltub see profiili edukast juurutamisest.

Esialgne taristu häälestamine ja sellega seotud kliendiserdi profiili konfiguratsioon nõuavad sageli tõrkeotsingut. Juhised NDES-konnektori eduka häälestamise ja tõrkeotsingujuhiste kohta serdijuurutusega seotud probleemide lahendamiseks leiate järgmisest teemast. 

- [Intune'i abil SCEP-i toe konfigureerimine](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Scep-serdiprofiilide tõrkeotsingu ülevaade Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Kasutage konfiguratsiooni kinnitamiseks viidatud powerShelli skripte. Lisateavet leiate teemast [Intune'i serdi konnektori kinnitusskriptid.](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)

  
**Muud levinumad probleemid**

**Kui proovite installida Intune'i serdi konnektorit NDES-konnektoriserverisse, kuvatakse teade "Serditaotluse parooli ei saa kontrollida. Võimalik, et seda on juba kasutatud. Hankige selle taotlusega esitamiseks uus parool."**  

See teade tähendab, et peate käivitama serdi konnektori installimise administraatorina.

Mõnes keskkonnas peavad Intune'iga ühenduse loomiseks kasutama puhverserverit serverid, kus Intune'i sert töötab, ja seega peab serdi konnektor kasutama puhverserverit. Mõnel juhul eirab NDES-konnektor konfigureeritud puhverserveri sätteid ja võib-olla on vaja konfigureerida puhverserveri sätted localSystemi turbekontekstis. 
 
Lahendus on käivitada Internet Explorer süsteemina ja konfigureerida puhverserveri IE-s. Pärast Intune'i konnektoriteenuse taaskäivitamist loob NDES-konnektor ühenduse Intune'iga.

**Kasutajaseadmed ei saa enam SCEP-serte NDES-ilt.**

On võimalik, et NDES-serverile välja antud ja NDES-i konnektori installimisel määratud kliendiautentimise sert on aegunud või puudub. Probleemi lahendamiseks: 
 
1. Desinstallige NDES-konnektor.  
2. Nende üksikasjade abil saate taotleda uut kliendiautentimist või serveri autentimiserti. 
 
    - Teema nimi: CN=external fqdn  
    - Teema alternatiivne nimi (mõlemad on nõutavad): DNS=external fqdn, DNS=internal fqdn 
 
3. Installige NDES-konnektor uue serdiga uuesti.