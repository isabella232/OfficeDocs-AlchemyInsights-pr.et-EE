---
title: Probleemid makromajandusliku finantsabi
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36545158"
---
# <a name="issues-with-mfa"></a>Probleemid makromajandusliku finantsabi
On paar asja kontrollida, kui kasutajad ei saa sisse logida, kasutades mitme teguriga autentimine (MFA)

1. Mõjutatud kasutaja võib blokeerida Azure Active Directory keskkonnas. Kui see juhtub, autentimise katsed selleks keelatakse automaatselt konkreetse kasutaja. [Palun järgige selles artiklis endi blokeerimise lõpetamist.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Kui kasutaja on blokeeritud või blokeeringu kasutaja ei aidanud proovige lähtestada kasutaja MFA ja nad lähevad läbi registreeruda protsessi uuesti. [Palun järgige selles artiklis.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Kui esimest korda te lubatud MFA ja kasutajad ei saa logida-brauserid kliendid, nagu Outlook, Skype jne, ehk ADAL (Active Directory autentimise Raamatukogu) on sisse lülitatud tellimuse O365. Sel juhul peate ühendust Exchange Online PowerShelli ja käivitada:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*