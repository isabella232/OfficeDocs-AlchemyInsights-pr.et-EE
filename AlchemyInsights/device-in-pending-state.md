---
title: Seade ootel olekus
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/11/2020
ms.locfileid: "49677571"
---
# <a name="device-in-pending-state"></a>Seade ootel olekus

**Eeltingimused**

1. Kui häälestate seadme registreerimisi esimest korda, veenduge, et olete üle vaadanud rakenduse [Azure Active Directory (AZURE ad) seadmete halduse tutvustuse](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) , mis juhendab teid, kuidas hankida seadmeid Azure AD ' i kontrolli all.
2. Kui registreerite seadmeid Azure AD otse ja registreerite need Intune ' i, peate veenduma, et olete [konfigureerinud Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) ' i ja lubama kõigepealt [litsentsimise](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) .
3. Veenduge, et teil on lubatud sooritada toiminguid Azure AD ' is ja kohapealses REKLAAMIs. Ainult Azure AD globaalne administraator saab seadme registreerimiste sätteid hallata. Kui häälestate automaatseid registreerimisi asutusesiseses Active Directorys, peate olema Active Directory ja AD FS-i administraator (kui see on olemas).

Hübriid-Azure AD liitumise registreerimise protsess eeldab, et seadmed on ettevõtte võrgus. See toimib ka VPN-i kaudu, kuid selle jaoks on mõned piirangud. Oleme kuulnud kliente, kes vajavad abi hübriid-Azure AD joini registreerimise protsessis serveri töö tingimustes.

**Pilvepõhise autentimise keskkond (Azure AD Password Hash Synci või läbitud autentimise abil)**

Seda registreerimis voog on tuntud ka kui "Sünkrooni Liitu".

Järgnevalt on toodud, mis juhtub registreerimise käigus.

1. Windows 10 avastab teenuse liitumispunkti (SCP) kirje, kui kasutaja logib seadmesse sisse.

    1. Seade proovib kõigepealt rentniku teavet, mis on pärit kliendipoolse SCP-i registrist [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Lisateavet leiate teemast [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Kui see ei õnnestu, suhtleb seade kohapealse Active Directoryga, et saada SCP-ist teavet rentniku kohta. SCP-i kinnitamiseks viidake sellele [dokumendile](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > Soovitame teha aktiivses kataloogis SCP ja kasutada ainult kliendipoolse SCP-i algseks kinnitamiseks.

2. Windows 10 proovib Azure AD-ga suhelda süsteemi kontekstis, et autentida ennast Azure AD vastu.

    Saate kontrollida, kas seadmel on süsteemi konto kaudu juurdepääs Microsofti ressurssidele, kasutades funktsiooni [test Device registreerimine ühenduvuse skripti](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 genereerib iseallkirjastatud serdi ja talletab selle arvuti objekti all asutusesiseses Active Directorys. See eeldab, et domeenikontroller on vaateväljas.

4. Seadme objekt, mis sisaldab serti, sünkroonitakse Azure AD-ga Azure AD Connecti kaudu. Sünkroonimise tsükkel on vaikimisi iga 30 minuti järel, kuid sõltub Azure AD Connecti konfiguratsioonist. Lisateavet leiate sellest [dokumendist](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. Praeguses etapis peaks teil olema võimalus vaadata teema seadet jaotises "**Ootel**" olekus Azure ' i portaalis Device Blade.

6. Järgmise kasutaja sisselogimise korral versioonile Windows 10 on registreerimine lõpule viidud.

    > [!NOTE]
    > Kui kasutate VPN-i ja väljalogimine/logimine lõpetab domeeni ühenduvuse, saate käivitada registreerimise käsitsi. Selleks tehke järgmist.
    >
    > Väljastage `dsregcmd /join` kohalikult administraatori viip või PSExec kaudu arvuti kaudu.
    >
    > Näiteks: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Azure Active Directory seadme registreerimisega seotud levinumate probleemide kohta leiate teavet teemast [seadmete KKK](https://docs.microsoft.com/azure/active-directory/devices/faq).
