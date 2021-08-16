---
title: Probleemid MFA-ga
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: b39c79063c66ea41585c8f9eec372bfac77bc0aa29ded5a5572e06c141b28f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098598"
---
# <a name="issues-with-azure-mfa"></a>Azure'i MFA probleemid
On paar asja, mida kontrollida, kas kasutajad ei saa mitme teguriga autentimise (MFA) abil sisse logida

1. Mõjutatud kasutaja võidakse blokeerida Azure Active Directory portaalis. Sel juhul keelatakse selle konkreetse kasutaja autentimiskatsed automaatselt. [Nende blokeeringu tühistamiseks järgige selles artiklis toodud juhiseid.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Kui kasutaja blokeeringu tühistamisest polnud abi või kasutaja pole blokeeritud, võite proovida kasutaja jaoks MFA lähtestada ja ta läbib registreerumise uuesti. [Järgige selles artiklis toodud juhiseid.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Kui lubate MFA esimest korda ja teie kasutajad ei saa sisse logida brauserivälistesse klientidesse (nt Outlook, Skype jne), siis võib-olla pole teie O365 tellimuses lubatud ADAL (Active Directory autentimisteek). Sel juhul peate powershelliga ühenduse Exchange Online käivitama: *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*