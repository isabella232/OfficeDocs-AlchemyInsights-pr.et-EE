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
ms.openlocfilehash: d16389ca577970deaf743255f75dc86134e79dcab2fff8c33987532fc7ee1105
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890430"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>SMTP-autentimise ja tõrkeotsingu lubamine

Kui soovite postkasti jaoks lubada SMTP-autentimise või saate tõrke "Klient pole autenditud", "Autentimine nurjus" või "SmtpClientAuthentication" koodiga 5.7.57 või 5.7.3 või 5.7.139, kui proovite meilisõnumit edastada seadme või rakenduse Microsoft 365 abil, tehke probleemi lahendamiseks järgmist kolme toimingut.

1. Keelake [Azure'i turbe vaikesätted,](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) kui soovite lubada turbe **vaikesäteteks** **Ei.**

    a. Logige Azure'i portaali sisse turbeadministraatori, tingimusjuurdepääsu administraatori või üldadministraatorina.<BR/>
    b. Liikuge sirvides Azure Active Directory > **atribuutideni.**<BR/>
    c. Valige **Halda turbe vaikesätet**.<BR/>
    d. Määrake **väärtuse Luba turbe vaikesätted** väärtuseks **Ei**.<BR/>
    e. Valige **Salvesta**.

2. [Luba kliendi SMTP-edastus](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) litsentsitud postkastis.

    a. Valige Microsoft 365 halduskeskus Aktiivsed **kasutajad** ja valige kasutaja.<BR/>
    b. Avage vahekaart Meil ja valige jaotises **Meilirakendused** nupp **Halda meilirakendusi.**<BR/>
    d. Veenduge, **et autenditud SMTP** oleks märgitud (lubatud).<BR/>
    e. Valige **Salvesta muudatused**.<BR/>

3. [Keelake litsentsitud postkastis mitme teguriga autentimine (MFA).](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa)

    a. Avage Microsoft 365 halduskeskus ja valige vasakpoolses navigeerimismenüüs **Kasutajad**  >  **Aktiivsed kasutajad.**<BR/>
    b. Valige **Mitmikautentimine**.<BR/>
    c. Valige kasutaja ja keelake **mitme teguriga autentimine.**<BR/>
