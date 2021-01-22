---
title: SSO-ühendusega seotud probleemid
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "7810"
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935111"
---
# <a name="sso-connection-issues"></a>SSO-ühendusega seotud probleemid

1. Järgige Kiirjuhend: rakenduse konfigureerimiseks [rakenduste juhendi atribuutide konfigureerimine](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) .
2. Olenevalt teie valitud rakendusest ja [ühekordsest sisselogimise suvandist](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) järgige allpool olevaid asjakohaseid juhiseid.
    - **Kohapealse rakenduse** konfigureerimiseks **SAML ühekordse sisselogimise** jaoks lugege teemat kohapealsete [rakenduste SAML rakenduse puhverserveriga](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).
    - **Parooli alusel ühekordse sisselogimise** **pilve rakenduse** konfigureerimiseks vaadake teemat [parooli ühekordse sisselogimise konfigureerimine](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).
    - **Kohapealse rakenduse** konfigureerimiseks **ühekordse sisselogimise rakenduse puhverserveri kaudu** leiate teavet teemast [paroolide häälestamine ühekordse sisselogimise jaoks rakenduse puhverserveriga](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
3. **Rakenduse puhverserveri probleemide tõrkeotsing**: Soovitame alustada läbivaatust tõrkeotsingu voo, [siluda rakenduse puhverserveri konnektori probleeme](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), et kindlaks teha, kas rakenduse puhverserveri konnektorid on õigesti konfigureeritud. Kui teil on endiselt probleeme rakendusega ühenduse loomisega, järgige rakenduse [puhverserveri rakenduse puhverserveri tõrkeotsing probleeme](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). [Cors probleeme saate tuvastada](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) brauseri silumise tööriistade abil.
    - Käivitage brauser ja liikuge sirvides veebi rakendusse.
    - Debug konsooli kuvamiseks vajutage klahvi **F12** .
    - Proovi reprodutseerida tehing ja vaadata konsooli sõnum. CORS rikkumine tekitab konsooli tõrke päritolu kohta.
    - Mõnda CORS probleemi ei saa lahendada (nt kui teie rakendus suunab autentimiseks login.microsoft.com ja juurdepääsuluba aegub). CORS kõne nurjub. Selle stsenaariumi lahendus on pikendada juurdepääsuluba, et takistada selle kehtivust kasutaja seansi ajal. Lisateavet selle kohta leiate teemast [Konfigureeritav turbelubade eluiga Microsoft Identity Platform ' is](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. **SAML põhinev Ühekordne sisselogimine**: soovitame kontrollida probleeme, mis [logivad sisse SAML-põhisesse ühekordse sisselogimise konfigureeritud rakendusse](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery), et leida lahendused probleemidele, mida tõenäoliselt tõenäoliselt koged.
5. **Parool põhinev Ühekordne sisselogimine**: soovitame kontrollida [Azure AD ' is parooli põhise ühekordse sisselogimise tõrkeotsingut](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso), et leida lahendused probleemidele, mida tõenäoliselt kogete.
6. Lisateavet VPN-i kasutamise ajal leiate teemast [ühekordse sisselogimise (SSO) kasutamine VPN-i ja Wi-Fi ühenduste kaudu](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections).
