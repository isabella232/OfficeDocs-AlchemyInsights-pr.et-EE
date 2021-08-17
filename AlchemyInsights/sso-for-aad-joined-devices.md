---
title: Single-Sign ühendatud Azure Active Directory jaoks sisse
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: 365225926296677feb7853481651a634792fd8bfa9abd9dc9359ffaae50b60eb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050006"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Ühekordne sisselogimine Azure Active Directory seadmete jaoks

Kui teil on kohapealne Active Directory (AD) keskkond ja soovite liituda oma AD domeeniga ühendatud arvutitega Azure AD-ga, saate seda teha azure AD-hübriidjuurutuse abil. [Juhised. Hübriidjuurutuse plaanimine Azure Active Directory juurutamine](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) pakub teile seotud juhiseid Azure AD hübriidjuurutuse juurutamiseks oma keskkonnas.

[Azure AD-ga ühendatud seadmete konfigureerimine asutusesiseseks Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Primaarse värskendamise loaga (PRT) seotud probleemid** Primaarne värskendustõend (PRT) on Azure AD autentimise põhiartiifakt Windows 10, Windows Server 2016 ja uuemates versioonides, iOS-is ja Androidi seadmetes. See on JSON Web Token (JWT), mis on spetsiaalselt välja antud Microsofti esimese osapoole loamaakleritele, et võimaldada ühekordset sisselogimist (SSO) kõigis nendes seadmetes kasutatavates rakendustes. Mis on [primaarvärskenduse luba?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)anname teada, kuidas PRT-d välja antakse, kasutatakse ja Windows 10 kaitsta.

**WamDefaultSet: YES ja AzureADPrt: YES** Need väljad näitavad, kas kasutaja on seadmesse sisselogimisel Azure AD-ga autenditud. Kui väärtused on **NO,** võib selle tähtaeg olla järgmine.

- Seadmega registreerumisel seostatud TPM-i halb salvestusvõti (kontrollige administraatoriõigustes töötades klahvisignTesti).
- Alternatiivne sisselogimistunnus
- HTTP-puhverserverit ei leitud

Seadmete tõrkeotsing käsu dsregcmd abil – [SSO olek](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
