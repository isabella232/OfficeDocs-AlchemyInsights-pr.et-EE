---
title: Single-Sign Active Directoryga ühendatud seadmete jaoks
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
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404591"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Ühekordne sisselogimine Azure Active Directory liidetud seadmete jaoks

Kui teil on kohapealne Active Directory (AD) keskkond ja soovite liituda oma AD domeeniga ühendatud arvutitega Azure AD-ga, saate seda teha azure AD-hübriidjuurutuse abil. [Juhised. Azure Active Directory hübriidjuurutuse plaanimine](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) pakub teile seotud juhiseid Azure AD hübriidjuurutuse juurutamiseks oma keskkonnas.

[Azure AD-ga ühendatud seadmete konfigureerimine Single-Sign Windows Hello for Businessi abil](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Primaarse värskendamise loaga (PRT) seotud probleemid** Primaarne värskendustõend (PRT) on Windows 10, Windows Server 2016 ja uuemate versioonide, iOS-i ja Androidi seadmete Azure AD-autentimise põhiartist. See on JSON Web Token (JWT), mis on spetsiaalselt välja antud Microsofti esimese osapoole loamaakleritele, et võimaldada ühekordset sisselogimist (SSO) kõigis nendes seadmetes kasutatavates rakendustes. [In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)( Mis on esmane värskendustõend?) anname teada, kuidas PRT-d windows 10 seadmetes välja antakse, kasutatakse ja kaitstakse.

**WamDefaultSet: YES ja AzureADPrt: YES** Need väljad näitavad, kas kasutaja on seadmesse sisselogimisel Azure AD-ga autenditud. Kui väärtused on **NO,** võib selle tähtaeg olla järgmine.

- Seadmega registreerumisel seostatud TPM-i halb salvestusvõti (kontrollige administraatoriõigustes töötades klahvisignTesti).
- Alternatiivne sisselogimistunnus
- HTTP-puhverserverit ei leitud

Seadmete tõrkeotsing käsu dsregcmd abil – [SSO olek](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
