---
title: SSO-ühenduse probleemid
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
ms.openlocfilehash: 8fb93bc40c6cd5a7c0e3d259fe3be8d1bab3187dd5aa023eb49977555fd930de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084342"
---
# <a name="sso-connection-issues"></a>SSO-ühenduse probleemid

1. Rakenduse [konfigureerimiseks järgige quickstart:](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) konfigureerige rakendusejuhendi atribuudid.
2. Olenevalt valitud rakendusest ja ühekordse sisselogimise [suvandist](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) järgige alltoodud juhiseid.
    - **SAML-i-põhise** ühekordse sisselogimise jaoks asutusesisese rakenduse konfigureerimiseks lugege teemat SAML-i ühekordne sisselogimine rakenduse [puhverserveriga kohapealste rakenduste jaoks.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
    - Pilverakenduse **konfigureerimiseks** **paroolipõhise ühekordse** sisselogimise jaoks lugege teemat [Parooli ühekordse sisselogimise konfigureerimine.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - Rakenduse puhverserveri **kaudu** ühekordse sisselogimise jaoks asutusesisese rakenduse konfigureerimise kohta leiate lisateavet teemast Ühekordse sisselogimise paroolhoidla rakenduse [puhverserveriga](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
3. **Rakenduse puhverserveri probleemide tõrkeotsing.** Soovitame alustada tõrkeotsinguvoo ülevaatamist, [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)rakenduse puhverserveri konnektori probleemide silumist, et teha kindlaks, kas rakenduse puhverserveri konnektorid on õigesti konfigureeritud. Kui teil on endiselt probleeme rakendusega ühenduse loomisega, järgige tõrkeotsinguvoogu rakenduses Rakenduse puhverserveri rakenduse probleemide [silumine.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) [CORS-i probleemide tuvastamiseks](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) saate kasutada brauseri silumistööriistu.
    - Käivitage brauser ja liikuge sirvides veebirakenduseni.
    - Silumiskonsooli säästmiseks vajutage klahvi **F12.**
    - Proovige tehing taasesitada ja vaadake konsooliteade läbi. CORS-i rikkumine annab lähtekohta konsoolivea.
    - Mõnda CORS-i probleemi ei saa lahendada (nt kui teie rakendus login.microsoft.com autentimiseks ümber ja juurdepääsuluba aegub). SEEJÄREL NURJUB CORS-kõne. Selle stsenaariumi lahendus on pikendada juurdepääsuluba, et takistada selle aegumist kasutaja seansi ajal. Lisateavet selle kohta leiate teemast Konfigureeritava loa kasutusajad [Microsofti identimisplatvorm](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. **SAML-i-põhise** ühekordse sisselogimise tõrkeotsing. Soovitame kontrollida, kas [SAML-i-põhisesse](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)ühekordse sisselogimisega rakendustesse sisselogimisel ilmnevad probleemid, et leida lahendused probleemidele, millega kõige tõenäolisemalt kokku puutute.
5. **Paroolipõhise ühekordse sisselogimise** tõrkeotsing. Soovitame kontrollida teemat Paroolipõhise ühekordse sisselogimise tõrkeotsing [Azure AD-s,](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)et leida lahendused probleemidele, millega kõige tõenäolisemalt kokku puutute.
6. Vpn-i kasutamise ajal ühendusega seotud probleemide kohta leiate teavet teemast Ühekordse sisselogimise [(SSO)](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)kasutamine VPN-i ja Wi-Fi kaudu.
