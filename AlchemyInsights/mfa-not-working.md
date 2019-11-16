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
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768833"
---
# <a name="issues-with-azure-mfa"></a>Probleemid Azure MFA
On mõned asjad, mida kontrollida, kui kasutajad ei saa sisse logida, kasutades mitme teguriga autentimine (MFA)

1. Mõjutatud kasutaja võib blokeerida Azure Active Directory portaalis. Kui see on nii, keelatakse autentimise katsed selle konkreetse kasutaja automaatselt. [Palun järgige käesoleva artikli juhiseid blokeeringu tühistamiseks.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Kui kasutaja blokeerimine ei aita või kasutaja ei ole blokeeritud võite proovida lähtestada kasutaja MFA ja nad lähevad läbi registreeruda protsessi uuesti. [Palun järgige käesoleva artikli juhiseid.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Kui see on esimene kord, kui aktiveerite MFA ja kasutajad ei saa sisse logida mitte-brauserid klientidele nagu Outlook, Skype, jne, võib-olla ADAL (Active Directory autentimine Raamatukogu) on lubatud teie O365 tellimus. Sel juhul peate ühendust Exchange Online PowerShelli ja käivitage see cmdlet-käsu:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*