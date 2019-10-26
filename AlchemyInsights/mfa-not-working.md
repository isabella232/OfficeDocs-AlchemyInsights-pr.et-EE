---
title: Makromajandusliku finantsabi probleemid
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/25/2019
ms.locfileid: "36545158"
---
# <a name="issues-with-mfa"></a>Makromajandusliku finantsabi probleemid
On mõned asjad, mida kontrollida, kui kasutajad ei saa sisse logida, kasutades mitme teguriga autentimine (MFA)

1. Mõjutatud kasutaja võib blokeerida Azure Active Directory portaalis. Kui see on nii, keelatakse autentimise katsed selle konkreetse kasutaja automaatselt. [Palun järgige käesoleva artikli juhiseid blokeeringu tühistamiseks.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Kui kasutaja blokeerimine ei aita või kasutaja ei ole blokeeritud võite proovida lähtestada kasutaja MFA ja nad lähevad läbi registreeruda protsessi uuesti. [Palun järgige käesoleva artikli juhiseid.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Kui see on esimene kord, kui aktiveerite MFA ja kasutajad ei saa sisse logida mitte-brauserid klientidele nagu Outlook, Skype, jne, võib-olla ADAL (Active Directory autentimine Raamatukogu) on lubatud teie O365 tellimus. Sel juhul peate ühendust Exchange Online PowerShelli ja käivitage see cmdlet-käsu:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*