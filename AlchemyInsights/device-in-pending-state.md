---
title: Seade on ootel olekus
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
ms.openlocfilehash: 224e6e613c306b50e354930bcbe6f43f1c08528766cb6e681b0e9826b2d55a4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53913999"
---
# <a name="device-in-pending-state"></a>Seade on ootel olekus

**Eeltingimused.**

1. Kui häälestate seadme registreerimisi esimest korda, veenduge, et olete läbi vaadanud [rakenduse Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) seadmehalduse tutvustuse, mis juhendab teid azure AD juhtimise all seadmete toomiseks.
2. Kui registreerite seadmeid otse Azure AD-sse ja registreerite need Intune'i, peate tagama, et [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) olete [Intune'i](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) konfigureerinud ja litsentsimise esmalt paika sidnud.
3. Veenduge, et teil oleks lubatud teha toiminguid Azure AD-s ja kohapeal AD-s. Seadmeregistreerimiste sätteid saab hallata ainult Azure AD üldadministraator. Kui häälestate automaatseid registreerimisi oma kohapealses Active Directorys, peate lisaks olema ka Active Directory ja AD FS-i (kui see on asjakohane) administraator.

Azure AD-ga liitumise hübriidjuurutuse registreerimine nõuab, et seadmed oleks ettevõtte võrgus. See toimib ka VPN-i kaudu, kuid selles on mõned piirangud. Oleme kuulnud, et kliendid vajavad abi Azure AD hübriidühenduse registreerimise tõrkeotsingul kaugtöö tingimustes.

**Pilvautentimise keskkond (Azure AD parooli hash-sünkroonimise või läbimise autentimine)**

Seda registreerimisvoogu nimetatakse ka "Sync Joiniks".

Siin on jaotus selle kohta, mis toimub registreerimise käigus.

1. Windows 10 tuvastab teenuseühenduspunkti (SCP) kirje, kui kasutaja seadmesse sisse logib.

    1. Seade proovib esmalt tuua rentnikuteavet kliendipoolsest SCP-st registris [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Lisateavet leiate teemast [Dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Kui see nurjub, suhtleb seade kohapealse Active Directoryga, et saada rentnikuteavet SCP-st. SCP kinnitamiseks vaadake seda [dokumenti.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)

    > [!NOTE]
    > Soovitame lubada SCP Active Directorys ja kasutada esmaseks valideerimiseks ainult kliendipoolset SCP-d.

2. Windows 10 azure AD-ga süsteemi kontekstis suhelda, et end Azure AD vastu autentida.

    Saate kontrollida, kas seade pääseb microsofti ressurssidele juurde süsteemikonto kaudu, kasutades seadme [registreerimise ühenduvuse testimisskripti.](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)

3. Windows 10 loob ise allkirjastatud serdi ja talletab selle arvutiobjekti all asutusesiseses Active Directorys. Selleks on vaja domeenikontrolleri vaatevälja.

4. Serdiga seadmeobjekt sünkroonitakse Azure AD-ga Azure AD Ühendus. Sünkroonimistsükkel on vaikimisi iga 30 minuti järel, kuid see sõltub Azure AD Ühendus. Lisateavet leiate sellest [dokumendist.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. Selles etapis peaks teemaseade olema näha olekus **"Ootel"** jaotises Azure'i portaali seadme laba.

6. Järgmisel kasutaja sisselogimisel Windows 10 registreerimine lõpule viidud.

    > [!NOTE]
    > Kui kasutate VPN-i ja sisselogimine/sisselogimine lõpetab domeeni ühenduvuse, saate registreerimise käivitada käsitsi. Selleks tehke seda.
    >
    > Probleem `dsregcmd /join` kohalikult administraatori viipa või kaugjuurdepääsu kaudu PSExec arvutisse.
    >
    > Näiteks: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Levinumad probleemid seadme Azure Active Directory leiate teemast [Seadmete KKK.](https://docs.microsoft.com/azure/active-directory/devices/faq)
