---
title: SMTP-autentimise ja tõrkeotsingu lubamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: f6f0228f6cdf7e07c9f439c54a7a2bd5364381c0e47dc80117bd964c5eafea61
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957204"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>SMTP-autentimise ja tõrkeotsingu lubamine

Kui soovite postkasti jaoks lubada SMTP-autentimise või saate tõrke "Klient pole autenditud", "Autentimine nurjus" või "SmtpClientAuthentication" koodiga 5.7.57 või 5.7.3 või 5.7.139, kui proovite meilisõnumit edastada, autentides seadme või rakenduse Microsoft 365 abil, tehke probleemi lahendamiseks järgmist kolme toimingut.

1. Keelake [Azure'i turbe vaikesätted,](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) kui soovite lubada turbe **vaikesäteteks** **Ei.**

    a. Logige Azure'i portaali sisse turbeadministraatori, tingimusjuurdepääsu administraatori või üldadministraatorina.<BR/>
    b. Liikuge sirvides Azure Active Directory > **atribuutideni.**<BR/>
    c. Valige **Halda turbe vaikesätet**.<BR/>
    d. Määrake **väärtuse Luba turbe vaikesätted** väärtuseks **Ei**.<BR/>
    e. Valige **Salvesta**.

2. [Luba kliendi SMTP-edastus](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) litsentsitud postkastis.

    a. Avage Microsoft 365 halduskeskus Aktiivsed **kasutajad** ja valige kasutaja.<BR/>
    b. Avage vahekaart Meil ja valige jaotises **Meilirakendused** nupp **Halda meilirakendusi.**<BR/>
    d. Veenduge, **et autenditud SMTP** oleks märgitud (lubatud).<BR/>
    e. Valige **Salvesta muudatused**.<BR/>

3. [Keelake litsentsitud postkastis mitme teguriga autentimine (MFA).](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa)

    a. Avage Microsoft 365 halduskeskus ja valige vasakpoolses navigeerimismenüüs **Kasutajad**  >  **Aktiivsed kasutajad**.<BR/>
    b. Valige **Mitmikautentimine**.<BR/>
    c. Valige kasutaja ja keelake **mitme teguriga autentimine.**<BR/>
