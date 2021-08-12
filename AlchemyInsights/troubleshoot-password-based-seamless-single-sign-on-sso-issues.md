---
title: Paroolipõhise sujuva ühekordse sisselogimise (SSO) probleemide tõrkeotsing
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
- "9004357"
- "9374"
ms.openlocfilehash: 6b4d7335461c913a6b5f782756684c5526a96c58c44853ddf9154aa51607bd4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972820"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Paroolipõhise sujuva ühekordse sisselogimise (SSO) probleemide tõrkeotsing

Paroolipõhise SSO põhitõdede kohta leiate teavet teemast [Paroolipõhine](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)autentimine Azure Active Directory .

**Paroolipõhise SSO konfigureerimine**

1. [Paroolipõhise ühekordse sisselogimise konfigureerimine –](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) selles artiklis kirjeldatakse täpsemalt paroolipõhist SSO-d. Kui lisatav rakendus nõuab kohandatud konfiguratsiooni ja peate kasutama paroolipõhist SSO-d, on see artikkel teie jaoks.
2. [Paroolipõhise ühekordse sisselogimise konfigureerimine](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) valmisrakenduste jaoks – rakenduse puhverserver toetab mitut ühekordse sisselogimise režiimi. Paroolipõhine sisselogimine on mõeldud rakenduste jaoks, mis kasutavad autentimiseks kasutajanime/parooli kombinatsiooni. Kui konfigureerite oma rakenduse jaoks paroolipõhise sisselogimise, peavad teie kasutajad ühe korra sisse logima asutusesisesesse rakendusse. Seejärel salvestab Azure Active Directory sisselogimisteabe ja tagab selle automaatselt rakendusele, kui kasutajad sellele kaugjuurdepääsu pääsevad.
    - Peaksite rakenduse rakenduse puhverserveri abil juba avaldanud ja testima. Kui see pole nii, järgige juhiseid jaotises Rakenduste avaldamine [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) rakenduse puhverserveri abil ja jätkake oma paroolipõhise SSO konfigureerimist eelrakenduste jaoks.

Paroolipõhise SSO tõrkeotsingu kohta leiate teemast Paroolipõhise ühekordse sisselogimise tõrkeotsing [Azure AD-s](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
