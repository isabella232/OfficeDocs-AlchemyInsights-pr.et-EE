---
title: Azure AD liitunud seadmete ühekordse sisselogimise tõrkeotsing
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035467"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Azure AD liitunud seadmete ühekordse sisselogimise tõrkeotsing

Kui teil on kohapealne Active Directory (AD) keskkond ja soovite liituda oma AD domeeniga liitunud arvutitega Azure AD-ga, saate selle saavutamiseks kasutada hübriid Azure AD Liitu. [Kuidas: teie hübriid-Azure Active Directory liitumise kavandamine](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) annab teile sellega seotud juhised hübriid-Azure AD joini rakendamiseks teie keskkonnas.

Lisateavet leiate teemast [AZURE ad liitunud seadmete konfigureerimine kohapealsete Single-Sign jaoks Windows Hello for δri abil](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).

**Esmase värskendamise turbelubade (PRT) probleemid**

Esmane värskendussagedus (PRT) on Windows 10, Windows Server 2016 ja uuemates versioonides, iOS-i ja Androidi seadmetes Azure AD autentimise peamine artefakt. See on JSON-veebimärk (JWT), mis on spetsiaalselt välja antud Microsoft First Party turbelubade vahendajatele, et lubada ühekordse sisselogimise (SSO) kasutamist nendes seadmetes kasutatavates rakendustes. Lisateavet selle kohta, kuidas PRT on Windows 10 seadmetes välja antud, kasutatud ja kaitstud, leiate teemast [mis on esmane värskendatav märk?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: Jah ja AzureADPrt: Jah**

Need väljad näitavad, kas kasutaja on seadmesse sisselogimisel Azure AD-sse autentinud. Kui väärtused on **ei**, võib selle põhjus olla järgmine.

- Vigane salvestusseade, mis on seadmega seotud TPM-iga registreerimisel (Kontrollige KeySignTest töötamise ajal)
- Alternatiivne sisselogimise ID
- HTTP puhverserverit ei leitud

Dsregcmd käsuga seadmete tõrkeotsingu kohta leiate teavet artiklist [SSO olek](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).
