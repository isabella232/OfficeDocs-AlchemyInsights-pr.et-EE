---
title: Azure AD-ga ühendatud seadmete ühekordse sisselogimise tõrkeotsing
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
ms.openlocfilehash: 872333e13bb51b3a22431154627ad561f6db88c681c9eeee523fdd09e58c0371
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039242"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Azure AD-ga ühendatud seadmete ühekordse sisselogimise tõrkeotsing

Kui teil on kohapealne Active Directory (AD) keskkond ja soovite liituda oma AD domeeniga ühendatud arvutitega Azure AD-ga, saate seda teha azure AD-hübriidjuurutuse abil. [Juhised. Hübriidjuurutuse plaanimine Azure Active Directory juurutamine](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) pakub teile seotud juhiseid Azure AD hübriidjuurutuse juurutamiseks oma keskkonnas.

Lisateavet leiate teemast [Azure AD-ga](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)ühendatud seadmete konfigureerimine asutusesiseseks Single-Sign On using Windows Hello for Business .

**Primaarse värskendamise loaga (PRT) seotud probleemid**

Primaarne värskendustõend (PRT) on Azure AD autentimise põhiartiifakt Windows 10, Windows Server 2016 ja uuemates versioonides, iOS-is ja Androidi seadmetes. See on JSON Web Token (JWT), mis on spetsiaalselt välja antud Microsofti esimese osapoole loamaakleritele, et võimaldada ühekordset sisselogimist (SSO) kõigis nendes seadmetes kasutatavates rakendustes. Lisateavet PRT väljastamis-, kasutatud ja kaitstud Windows 10 kohta leiate teemast Mis on esmane [värskendustõend?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: YES ja AzureADPrt: YES**

Need väljad näitavad, kas kasutaja on seadmesse sisselogimisel Azure AD-ga autenditud. Kui väärtused on **NO,** võib põhjuseks olla:

- Seadmega registreerumisel seostatud TPM-i halb salvestusvõti (kontrollige administraatoriõigustes töötades klahvisignTesti)
- Alternatiivne sisselogimistunnus
- HTTP-puhverserverit ei leitud

Seadmete tõrkeotsinguks käsu dsregcmd abil lugege [teemat SSO olek](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).
