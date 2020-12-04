---
title: PRT probleemi tõrkeotsing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573494"
---
# <a name="troubleshoot-prt-issue"></a>PRT probleemi tõrkeotsing

Kui soovite autentimine uuesti sooritada, peab see olema täielikult registreeritud ja heas olekus ning hankima esmase värskendamise tõendi (PRT).

Hübriid-Azure AD liitumise registreerimise protsess eeldab, et seadmed peavad olema ettevõtte võrgus. See toimib ka VPN-i kaudu, kuid selle jaoks on mõned piirangud. Oleme kuulnud kliente, kes vajavad abi seoses hübriid-Azure AD Jointi registreerimisega, mis on seotud Kaug-töö asjaoludega. Siin on jaotus, mis toimub "kapoti all" registreerimise käigus.

**Pilvepõhise autentimise keskkond (Azure AD Password Hash Synci või läbitud autentimise abil)**

Seda registreerimis voog on tuntud ka kui "Sünkrooni Liitu".

1. Windows 10 avastas SCP-kirje kasutaja sisselogimise korral seadmesse.
    1. Seade proovib kõigepealt rentniku teavet, mis on pärit kliendipoolse SCP-i registrist [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Lisateavet leiate sellest [dokumendist](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. Kui see ei õnnestu, suhtleb seade kohapealse Active Directoryga (AD), et saada rentniku teavet teenusest Connection Point (SCP). SCP-i kontrollimiseks lugege seda [dokumenti](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

> [!NOTE]
> Soovitame anda REKLAAMIle SCP ja kasutada seda ainult kliendipoolse SCP-i esmaseks kinnitamiseks.

2. Windows 10 proovib Azure AD-ga suhelda süsteemi kontekstis, et autentida ennast Azure AD vastu. Saate kontrollida, kas seadmel on süsteemi konto kaudu juurdepääs Microsofti ressurssidele, kasutades funktsiooni test Device registreerimine ühenduvuse skripti.

3. Windows 10 loob iseallkirjastatud serdi ja salvestab selle kohapeal asuvas arvutis asuvale objektile. See eeldab, et domeenikontroller on vaateväljas.

4. Seadme objekt, mis on serdi saab sünkroonida Azure AD kaudu Azure AD Connect. Sünkroonimise tsükkel on vaikimisi iga 30 minuti järel, kuid sõltub Azure AD Connecti konfiguratsioonist. Lisateavet leiate sellest [dokumendist](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. Praeguses etapis peaks teil olema võimalus vaadata teema seadet jaotises "ootel" olekus Azure ' i portaalis Device Blade.

6. Järgmise kasutaja sisselogimise korral versioonile Windows 10 on registreerimine lõpule viidud. 

> [!NOTE]
> Kui kasutate VPN-i ja väljalogimine – sisselogimise protsess katkestab domeeni ühenduvuse, saate käivitada registreerimise käsitsi.
 1. Väljastage dsregcmd/JOIN kohalikult administraatori viibale või PSExec kaudu teie ARVUTISSE. Näiteks PsExec-s \\ win10client01 cmd, dsregcmd/JOIN

 2. Lisateavet hübriidiga liitumise probleemide kohta leiate teemast [seadmete probleemi tõrkeotsing](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
