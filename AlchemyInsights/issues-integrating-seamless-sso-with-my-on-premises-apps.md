---
title: Tõrgeteta SSO integreerimise probleemid kohapealsete rakendustega
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868675"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Tõrgeteta SSO integreerimise probleemid kohapealsete rakendustega

Tõrgeteta SSO integreerimise probleemide lahendamiseks kohapealsete rakendustega tehke järgmist.

**Soovitatavad toimingud**

1. **Kohapealse rakenduse** konfigureerimiseks **ühekordse sisselogimise rakenduse puhverserveri kaudu** leiate teavet teemast [paroolide häälestamine ühekordse sisselogimise jaoks rakenduse puhverserveriga](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **Rakenduse puhverserveri probleemide tõrkeotsing**: Soovitame alustada läbivaatust tõrkeotsingu voo, [siluda rakenduse puhverserveri konnektori probleeme](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), et kindlaks teha, kas rakenduse puhverserveri konnektorid on õigesti konfigureeritud. Kui teil on endiselt probleeme rakendusega ühenduse loomisega, järgige tõrkeotsingu juhiseid rakenduses [debug rakenduse puhverserveri probleemid](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). [Cors probleemide tuvastamiseks](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) saate kasutada järgmisi brauseri debug tööriistu.
    1. Käivitage brauser ja liikuge sirvides veebi rakendusse.
    1. Debug konsooli kuvamiseks vajutage klahvi **F12** .
    1. Proovi reprodutseerida tehing ja vaadata konsooli sõnum. CORS rikkumine tekitab konsooli tõrke päritolu kohta.
    1. Mõnda CORS probleemi ei saa lahendada (nt kui teie rakendus suunab autentimiseks login.microsoftonline.com ja juurdepääsuluba aegub). CORS kõne nurjub. Selle stsenaariumi lahendus on pikendada juurdepääsuluba, et takistada selle kehtivust kasutaja seansi ajal. Lisateavet selle kohta leiate teemast [Konfigureeritav turbelubade eluiga Microsoft Identity Platform ' is](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Soovitatavad dokumendid**

- [Ühekordse sisselogimise konfigureerimine rakenduse puhverserveri rakendusse](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [SAML ühekordse sisselogimise rakendused rakenduse puhverserveriga](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Azure Active Directory rakenduse puhverserveri CORS probleemide mõistmine ja lahendamine](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Kerberose piiratud delegeerimise konfiguratsioonide tõrkeotsing rakenduse puhverserveri korral](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)