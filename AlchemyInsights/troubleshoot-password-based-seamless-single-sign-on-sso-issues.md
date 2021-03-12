---
title: Paroolil põhinevate tõrgeteta ühekordse sisselogimise (SSO) probleemide tõrkeotsing
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
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714767"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Paroolil põhinevate tõrgeteta ühekordse sisselogimise (SSO) probleemide tõrkeotsing

Parooli põhise SSO põhialuste kohta leiate teavet teemast [paroolide autentimine Azure Active Directory abil](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).

**Parooli põhise SSO konfigureerimine**

1. [Parooli põhise ühekordse sisselogimise konfigureerimine](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) – selles artiklis kirjeldatakse üksikasjalikumalt parooli põhise SSO suvandit. Kui lisatav rakendus vajab kohandatud konfiguratsiooni ja te peate kasutama parooli põhiset SSO-d, siis see artikkel on teie jaoks.
2. [Parooli põhise ühekordse sisselogimise konfigureerimine – Prem rakendused](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) – rakenduse puhverserver toetab mitmeid ühekordse sisselogimise režiime. Paroolil põhinev sisselogimine on mõeldud rakendustele, mis kasutavad autentimiseks kasutajanime/parooli kombinatsiooni. Kui konfigureerite oma rakenduse jaoks parooli-põhise sisselogimise, peavad kasutajad olema sisse logitud kohapealsesse rakendusse. Pärast seda salvestab Azure Active Directory sisselogimise teabe ja annab selle automaatselt rakendusele, kui kasutajad pääsevad sellele eemalt.
    - Sa peaksid juba avaldanud ja katsetanud oma rakendust rakenduse puhverserveriga. Kui ei, siis järgige rakenduse [Avalda rakendusi AZURE ad Application proxy abil](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) , seejärel jätkake oma parooli baasil kasutatava SSO häälestamist ka Prem-rakenduste jaoks.

Parooli põhise SSO tõrkeotsingu kohta leiate teavet teemast [parooli põhine ühekordne sisselogimise tõrkeotsing AZURE ad](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
