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
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810480"
---
# <a name="issues-with-azure-mfa"></a>Azure'i MFA probleemid
On paar asja, mida kontrollida, kas kasutajad ei saa mitme teguriga autentimise (MFA) abil sisse logida

1. Mõjutatud kasutaja võib olla Azure Active Directory portaalis blokeeritud. Sel juhul keelatakse selle konkreetse kasutaja autentimiskatsed automaatselt. [Nende blokeeringu tühistamiseks järgige selles artiklis toodud juhiseid.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Kui kasutaja blokeeringu tühistamisest polnud abi või kasutaja pole blokeeritud, võite proovida kasutaja jaoks MFA lähtestada ja ta läbib registreerumise uuesti. [Järgige selles artiklis toodud juhiseid.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Kui lubate MFA esimest korda ja teie kasutajad ei saa sisse logida brauserivälistesse klientrakendusse (nt Outlook, Skype jne), siis võib-olla pole teie O365 tellimuses lubatud ADAL (Active Directory autentimisteek). Sel juhul peate exchange Online'i PowerShelliga ühenduse loomiseks ja käivitama selle  *cmdlet-käsu: Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*