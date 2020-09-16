---
title: Probleemid MFA-ga
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755127"
---
# <a name="issues-with-azure-mfa"></a>Azure MFA probleemid
Kui kasutajad ei saa mitme teguri autentimise (MFA) abil sisse logida, on mitu võimalust.

1. Mõjutatud kasutaja võib olla blokeeritud Azure Active Directory portaalis. Kui see on nii, siis keeldutakse selle konkreetse kasutaja autentimise katsetest automaatselt. [Nende blokeeringu tühistamiseks järgige selle artikli juhiseid.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Kui kasutaja blokeeringu tühistamine ei aidanud või kasutaja ei ole blokeeritud, võite proovida lähtestada MFA kasutaja jaoks ja nad lähevad uuesti registreerumise protsessi. [Palun järgige selle artikli juhiseid.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Kui see on esimene kord, kui lubasite MFA ja kasutajad ei saa sisse logida mitte-brauserite klientidele (nt Outlook, skype jne), võib-olla ADAL (Active Directory autentimine teegis) pole teie O365 tellimusel lubatud. Sellisel juhul peate looma ühenduse Exchange Online PowerShelliga ja käivitama selle cmdlet-käsk:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*