---
title: Seadke ClientAccessServerEnabled väärtuseks True (Tõene).
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
ms.openlocfilehash: b134c952e3cc5305d8f3e6f44031e7f33d7938b67ff122c46cb74bbd33cbf59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994861"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Seadke ClientAccessServerEnabled väärtuseks True (Tõene).

Kui krüptitud meilisõnumit ei saa avada ja selle asemel kuvatakse **rpmsg-manus,** tehke järgmist.

1. Ühendus Exchange Online PowerShelli.

> [!NOTE]
> PowerShelliga ühenduse Exchange Online peate sisse logima üldadministraatori või administraatorikonto Exchange kaudu.

   a. Avage Windows PowerShell ja seejärel käivitage järgmine käsk.`$UserCredential = Get-Credential`
b. Sisestage **Windows PowerShell Identimisteabe** taotlus oma töö- või koolikonto ja parool c. Klõpsake nuppu **OK**. 

2. Uue seansi loomiseks käivitage järgmine käsk.

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Käivitage järgmine käsk:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Käsk `Get-IRMConfiguration` Käivita.

4. Kontrollige **sätet ClientAccessServerEnabled ( ClientAccessServerEnabled).** 

    a. Kui **sätte ClientAccessServerEnabled** väärtuseks on **seatud False (Väär),** käivitage järgmine cmdlet-käsk: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Sulgege powershelli seanss alati järgmise käsuga. `Remove-PSSession $Session`

Lisateavet leiate teemast [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

