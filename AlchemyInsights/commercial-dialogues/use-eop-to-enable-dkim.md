---
title: PowerShelli Exchange Online DKIM-i lubamine konkreetse domeeni jaoks
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: ba627c6da96624914b858aa09d6eff9de709134c2c986fe363845c5ab2b66434
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070292"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>PowerShelli Exchange Online DKIM-i lubamine konkreetse domeeni jaoks

Kui te ei saa halduskeskuses DKIM-i DNS-i kirjeid luua, proovige kasutada Exchange Online PowerShelli. 

PowerShelli abil DKIM-i DNS-Exchange Online loomiseks tehke järgmist.

1. Avage Windows PowerShell administraatorina ja käivitage kirjeldatud järjestuses järgmised käsud.

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Kui teil on PowerShelliga ühenduse Exchange Online probleeme, [lugege teemat Ühendus powershelli Exchange Online kohta.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. Kui olete PowerShelliga Exchange Online ühendatud, käivitage järgmine käsk.

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Kui ülaltoodud käsk on edukalt täidetud, käivitage PowerShelli seansi lõpetamiseks Exchange Online käsk:

    `Remove-PSSession $Session` 



