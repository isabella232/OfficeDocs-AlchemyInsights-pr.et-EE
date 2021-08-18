---
title: PRT-probleemi tõrkeotsing
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
ms.openlocfilehash: a005c4a6848bbf0725560375df1220ce906cbb5f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330955"
---
# <a name="troubleshoot-prt-issue"></a>PRT-probleemi tõrkeotsing

Selleks, et mis tahes seade saaks autendimise lõpule viia, peab see olema täielikult registreeritud ja heas olekus ning saama hankida primaarvärskenduse tõend (PRT).

Azure AD-ga liitumise hübriidjuurutuse registreerimine eeldab, et seadmed peavad olema ettevõtte võrgus. See toimib ka VPN-i kaudu, kuid selles on mõned piirangud. Oleme kuulnud, et kliendid vajavad abi Azure AD hübriidühenduse registreerimise tõrkeotsingul kaugtöö tingimustes. Siin on jaotus selle kohta, mis toimub registreerimise käigus "kapuutsi all".

**Pilvautentimise keskkond (Azure AD parooli hash-sünkroonimise või läbimise autentimine)**

Seda registreerimisvoogu nimetatakse ka "Sync Joiniks".

1. Windows 10 kasutaja seadmesse sisselogimisel SCP-kirje.
    1. Seade proovib esmalt tuua rentnikuteavet kliendipoolsest SCP-st registris [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Lisateavet leiate sellest [dokumendist.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)
    2. Kui see nurjub, suhtleb seade kohapealse Active Directoryga (AD), et saada rentnikuteavet teenuseühenduspunktist (SCP). SCP kinnitamiseks vaadake seda [dokumenti.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point) 

**Märkus.** Soovitame lubada SCP-d AD-s ja kasutada esmaseks valideerimiseks ainult kliendipoolset SCP-d.

2. Windows 10 azure AD-ga süsteemi kontekstis suhelda, et end Azure AD vastu autentida. Saate kontrollida, kas seade pääseb microsofti ressurssidele juurde süsteemikonto kaudu, kasutades seadme registreerimise ühenduvuse testimisskripti.

3. Windows 10 loob ise allkirjastatud serdi ja talletab selle asutusesiseseS AD-s arvutiobjekti all. Selleks on vaja domeenikontrolleri vaatevälja.

4. Serdiga seadmeobjekt sünkroonitakse Azure AD-ga Azure AD Ühendus. Sünkroonimistsükkel on vaikimisi iga 30 minuti järel, kuid see sõltub Azure AD Ühendus. Lisateavet leiate sellest [dokumendist.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. Selles etapis peaksite nägema teemaseadet olekus Ootel Azure'i portaali seadme laba all.

6. Järgmisel kasutaja sisselogimisel Windows 10 registreerimine lõpule viidud. 

**Märkus.** Kui kasutate VPN-i ja sisselogimisprotsess lõpetab domeeni ühenduvuse, saate registreerimise käivitada käsitsi.
 1. Probleem on dsregcmd /join locally on admin prompt or remotely via PSExec to your PC. Näiteks PsExec -s \\ win10client01 cmd, dsregcmd /join

 2. Lisateavet hübriidjuurutusprobleemide kohta leiate teemast [Seadmete probleemi tõrkeotsing.](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)
