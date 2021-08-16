---
title: Sujuva SSO ja minu kohapealste rakenduste integreerimisega seotud probleemid
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
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028288"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Sujuva SSO ja minu kohapealste rakenduste integreerimisega seotud probleemid

Tõrgeteta SSO integreerimise ja kohapealste rakendustega seotud probleemide tõrkeotsinguks tehke järgmist.

**Soovitatavad juhised**

1. Rakenduse puhverserveri **kaudu** ühekordse sisselogimise jaoks asutusesisese rakenduse konfigureerimise kohta leiate lisateavet teemast Ühekordse sisselogimise paroolhoidla rakenduse [puhverserveriga](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **Rakenduse puhverserveri probleemide tõrkeotsing.** Soovitame alustada tõrkeotsinguvoo [ülevaatamist,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)rakenduse puhverserveri konnektori probleemide silumist, et teha kindlaks, kas rakenduse puhverserveri konnektorid on õigesti konfigureeritud. Kui teil on endiselt probleeme rakendusega ühenduse loomisega, järgige tõrkeotsingu juhiseid jaotises Rakenduse puhverserverirakenduse probleemide [silumine.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) [CORS-i probleemide tuvastamiseks](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) saate kasutada järgmisi brauseri silumistööriistu.
    1. Käivitage brauser ja liikuge sirvides veebirakenduseni.
    1. Silumiskonsooli säästmiseks vajutage klahvi **F12.**
    1. Proovige tehing taasesitada ja vaadake konsooliteade läbi. CORS-i rikkumine annab lähtekohta konsoolivea.
    1. Mõnda CORS-i probleemi ei saa lahendada (nt kui teie rakendus login.microsoftonline.com autentimiseks ümber ja juurdepääsuluba aegub). SEEJÄREL NURJUB CORS-kõne. Selle stsenaariumi lahendus on pikendada juurdepääsuluba, et takistada selle aegumist kasutaja seansi ajal. Lisateavet selle kohta leiate teemast Konfigureeritava loa kasutusajad [Microsofti identimisplatvorm](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Soovitatud dokumendid**

- [Rakenduse puhverserveri rakenduse ühekordse sisselogimise konfigureerimine](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [SAML-i ühekordne sisselogimine rakenduse puhverserveri abil kohapealste rakenduste jaoks](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Rakenduse puhverserveri CORS Azure Active Directory probleemide mõistmine ja lahendamine](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Kerberose piiratud delegeerimiskonfiguratsioonide tõrkeotsing rakenduse puhverserveri jaoks](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)