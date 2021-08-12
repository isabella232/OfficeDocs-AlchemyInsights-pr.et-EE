---
title: 451 4.7.0 Ajutine serveritõrge. Proovige hiljem uuesti. PRX4
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2021
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "3000003"
- "12465"
ms.openlocfilehash: ce898981d053c8b5dc080ee83434bdacd7f02a636f0183293915bacdb48ba4ef
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812577"
---
# <a name="451-470-temporary-server-error-please-try-again-later-prx4"></a>451 4.7.0 Ajutine serveritõrge. Proovige hiljem uuesti. PRX4

Smarthosti "smtp.office365.com" kaudu meili saatmisel SMTP-kliendiedastuse meetodi abil võib ilmneda probleem ja teile kuvatakse tõrketeade "451 4.7.0 Temporary server error" (Ajutine serveritõrge). Proovige hiljem uuesti. PRX4 on enamasti ajutine." 

Veenduge, et te ei kasuta SMTP-kliendiedastuse jaoks ühispostkasti, kuna SMTP-kliendi edastusmeetod nõuab meilide saatmiseks litsentsitud postkasti. Kui te ühispostkasti ei kasuta ja probleem ei lahene, kontrollige järgmist.

1. Luba kliendi SMTP-edastus litsentsitud postkastis, kus seda PowerShelli käsku kasutatakse.

    ```Set-CASMailbox -Identity sean@contoso.com -SmtpClientAuthenticationDisabled $false```

    OR

    1. Avage Microsoft 365 halduskeskus > **Aktiivsed kasutajad** ja valige kasutaja.
    1. Avage menüü Meil > **Meilirakendused >** valige **Halda meilirakendusi.** 
    1. Veenduge, et **säte Autenditud SMTP** oleks märgitud (lubatud).
    1. Valige **Salvesta muudatused**.
    
    Smtp-autentimise lubamiseks terves asutuses käivitage järgmine käsk.

    `Set-TransportConfig -SmtpClientAuthenticationDisabled $true`
 
    **Märkus.** Turvalisuse huvides on soovitatav lubada SMTP-autentimine ainult kasutatava postkasti jaoks. Kasutajataseme säte alistab organisatsioonitaseme sätte.

2. Keelake Azure'i turbe vaikesätted, kui soovite lubada turbe **vaikesäteteks** **Ei.**

    1. Logige Azure'i portaali sisse turbeadministraatori, tingimusjuurdepääsu administraatori või üldadministraatorina.
    1. Liikuge sirvides Azure Active Directory >**  atribuutideni** ja valige **Halda turbe vaikesätet**.
    1. Seadke säte **Luba turbe vaikesätted** väärtuseks **Ei**.
    1. Valige **Salvesta**.

3. Keelake kasutatavas litsentsitud postkastis mitme teguriga autentimine (MFA).

    1. Avage Microsoft 365 halduskeskus ja valige vasakpoolses navigeerimismenüüs **Kasutajad**  >  **Aktiivsed kasutajad.**
    1. Valige lehel **Aktiivsed** kasutajad valik **Mitmikautentimine.**
    1. Valige kasutaja ja keelake **mitmikautentimine.**

