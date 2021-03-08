---
title: ClientAccessServerEnabled seadmine True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524559"
---
# <a name="set-clientaccessserverenabled-to-true"></a>ClientAccessServerEnabled seadmine True

Kui te ei saa krüptitud meilisõnumit avada ja selle asemel vaadata **rpmsg** manust, tehke järgmist.

1. Ühenduse loomine Exchange Online PowerShelliga.

> [!NOTE]
> Exchange Online PowerShelliga ühenduse loomiseks peate sisse logima üldise administraatori või Exchange ' i administraatori konto abil.

   loomine. Avage Windows PowerShell ja käivitage järgmine käsk. `$UserCredential = Get-Credential`
b. Sisestage dialoogiboksis **Windows PowerShelli mandaadi taotlus** oma töö-või kooli konto ja parool, c. Klõpsake nuppu **OK**. 

2. Uue seansi loomiseks käivitage järgmine käsk.

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    loomine. Käivitage järgmine käsk:
    
    `Import-PSSession $Session -DisableNameChecking`

3. `Get-IRMConfiguration`Käsk Käivita.

4. Märkige **ClientAccessServerEnabled** säte. 

    loomine. Kui **ClientAccessServerEnabled** säte on seatud väärtusele **FALSE**, käivitage järgmine cmdlet-käsk. `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Sulgege oma PowerShelli seanss alati järgmise käsuga: `Remove-PSSession $Session`

Lisateavet leiate teemast [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

