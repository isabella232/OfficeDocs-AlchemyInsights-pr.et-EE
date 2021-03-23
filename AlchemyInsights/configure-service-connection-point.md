---
title: Teenuse liitumispunkti konfigureerimine (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035451"
---
# <a name="configure-service-connection-point-scp"></a>Teenuse liitumispunkti konfigureerimine (SCP)

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **Põhjus**: SCP-objekti ei saa lugeda ja Azure AD rentniku teabe hankimine
- **Resolutsioon**: vaadake jaotist [teenuse liitumispunkti konfigureerimine](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**Tegevuskava**

- Kontrollige, kas seadmele on manustatud rühmapoliitika objekti, mida on kontrollitud.
- Veenduge, et rühmapoliitika GPO on loonud registrivõtmed.
- Veenduge, et teil oleks oma kataloogi ID ja onmicrosoft domeeniga loodud kaks võtit.

**Kliendipoolse registrisätete konfigureerimine SCP**

Järgmise näite abil saate luua rühmapoliitika objekti (GPO), et juurutada registri säte, mis konfigureerib teie seadmete registris SCP-kirje.

1. Avage rühmapoliitika halduskonsooli ja looge oma domeenis uus GPO.
     - Sisestage oma vastloodud GPO nimi (nt ClientSideSCP).

2. Redigeerige rühmapoliitika objekti ja otsige üles järgmine tee: **Arvuti konfiguratsioon > eelistused > Windowsi sätted > Registry**.

3. Paremklõpsake **registrit** ja valige **Uus > registri üksus**.

4. Konfigureerige vahekaardil **Üldine järgmine teave** .
  
- **Toiming**: värskendamine
    
- **Taru**: HKEY_LOCAL_MACHINE
    
- **Võtme tee**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Väärtuse nimi**: TenantId
    
- **Väärtuse tüüp**: REG_SZ
    
- **Value data**: Azure AD eksemplari GUID või kataloogi ID (selle väärtuse leiate **Azure ' i portaalist > azure Active Directory > atribuudid > kataloogi ID**)
 
- Klõpsake nuppu **OK**.
 
5. Paremklõpsake **registrit** ja valige **Uus > registri üksus**.

6. Konfigureerige vahekaardil **Üldine järgmine teave** .
  
- **Toiming**: värskendamine
    
- **Taru**: HKEY_LOCAL_MACHINE
    
- **Võtme tee**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Väärtuse nimi**: TenantName
    
- **Väärtuse tüüp**: REG_SZ
    
- **Value data**: teie kinnitatud domeeninimi, kui kasutate välise keskkonna (nt AD FS). Teie kinnitatud domeeninimi või teie onmicrosoft.com domeeninimi (nt contoso. onmicrosoft). com, kui kasutate hallatavat keskkonda

- Klõpsake nuppu **OK**.

7. Äsja loodud GPO redaktori sulgemine.

8. Lingi vastloodud GPO-ga soovitud OU sisaldavale domeeniga liitunud arvutitele, mis kuuluvad teie kontrollitava levikuga elanikkonnale.

Lisateavet leiate teemast [hübriid-AZURE ad Joint-AZURE ad kontrollitud valideerimine | Microsoft docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) ja  [tõrkeotsing hübriid-Azure Active Directory liitunud seadmed | Microsoft docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).









