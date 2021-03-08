---
title: Exchange Online PowerShelli kasutamine konkreetse domeeni DKIM lubamiseks
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
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524172"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Exchange Online PowerShelli kasutamine konkreetse domeeni DKIM lubamiseks

Kui te ei saa DKIM DNS-i kirjeid luua, proovige kasutada rakendust Exchange Online PowerShell. 

DKIM DNS-i kirje loomiseks Exchange Online PowerShelli abil tehke järgmist.

1. Avage Windows PowerShell administraatorina ja kasutage kirjeldatud järjestuses järgmisi käske.

    loomine. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Kui teil on Exchange Online PowerShelliga ühenduse loomisega probleeme, lugege teemat [ühenduse loomine Exchange Online PowerShelliga](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

2. Kui olete ühendatud Exchange Online PowerShelliga, käivitage järgmine käsk.

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Kui ülaltoodud käsk on edukalt täidetud, käivitage Exchange Online PowerShelli seansi lõpetamiseks järgmine käsk:

    `Remove-PSSession $Session` 



