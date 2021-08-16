---
title: Rakenduste konfigureerimine ja kohandamine
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
- "9004334"
- "7733"
ms.openlocfilehash: 3ce5b04469eb655c9d682f5830d9f906529aa40f706ee594b670708426d48769
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044984"
---
# <a name="configure-and-customize-applications"></a>Rakenduste konfigureerimine ja kohandamine

**Rakenduste konfigureerimine**

1. [Lühiülevaated. Rakenduse atribuutide konfigureerimine Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) rentnikus näitab, kuidas konfigureerida mõnda rakenduse atribuuti.
2. Teie rakenduste integreerimiseks Azure Active Directory välja töötatud õppematerjalid, [mis](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) aitavad teil konfiguratsioonis töötada.
3. [Rakenduse puhverserveri rakenduse konfigureerimine aitab](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) teil mõista, kuidas konfigureerida Azure AD-s rakenduse puhverserver, et teie asutusesisesed rakendused pilveteenusesse paljastada.
4. [Laadige alla PingAccess ja konfigureerige](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)rakendus. Järgige juhiseid jaotises *PingAccessi* konfigureerimine Azure AD-le, et kaitsta rakendusi, mis on avaldatud pingiidentiteedi veebisaidil Microsoft Azure AD Rakenduse puhverserver ja laadige alla PingAccessi uusim versioon.

**Valesti konfigureeritud rakenduse (AADSTS650056) tõrked**

1. Veenduge, et pääsete rakendusele juurde rakenduse omaniku esitatud sisselogimisaadressilt. Muul juhul tähendab see, et logige rakendusse sisse tavalise protsessi kaudu. Enamasti lahendatakse see automaatselt. Kui seda ei tee, aitab see postitus tõrkeotsingut ja probleemi lahendada.
2. **Kui rakendus kuulub teie ettevõttele** (see tähendab, et rakenduse registreerimine on teie ettevõttes):
    - Soovitame vähemalt Microsoft Graph `User.Read` `openid` delegeeritud  õigusi.
    - Veenduge, et rakendus ja kõik selle õigused on selleks nõusoleku saanud. Seda saate kontrollida, kui vaatate **API-õigustes** rakenduse registreerimise veergu **Olek.**
    - Mõnel juhul võib rakendus olla kolmandast osapoolest, kuid võib olla registreeritud teie asutuses. Kontrollige, kas see rakendus on teie rakenduse registreerimistes (mitte Enterprise'i rakendustes) loetletud.
    - Kui see tõrketeade kuvatakse ka edaspidi. Seejärel peate võib-olla 4. juhises **kirjeldatud nõusoleku URL-i üles ehitama.**
3. **Kui teie ettevõte pole rakenduse omanik ja kasutab seda kolmanda osapoole rakendusena,** siis:
    - Kui olete üld-/ettevõtteadministraator, peaksite nägema nõusoleku kuva. Veenduge, et märgite ruudu **"Consent on for your organization"**("Nõusolek ettevõtte nimel".
    - Kui te ei näe nõusolekukuva, kustutage Enterprise'i rakendus ja proovige uuesti.
    - Kui see tõrketeade kuvatakse ka edaspidi. Seejärel peate võib-olla 4. juhises **kirjeldatud nõusoleku URL-i üles ehitama.**
4. **Koostage kasutatav** nõusoleku URL käsitsi. Kui rakendus on loodud konkreetsele ressursile juurde pääsemiseks, ei pruugi teil olla võimalik Azure'i portaali nupud Nõusolek kasutada, peate ise ise oma nõusoleku URL-i genereerima ja seda kasutama.
    - Peate saama rakenduse omanikult selle ja `{App-Id}` `{App-Uri-Id}` selle. `{Tenant-Id}` on teie rentniku identifikaator. See on kas `yourdomain.onmicrosoft.com` teie kataloogi ID.
    - Kui rakendus pääseb ressursile juurde ise, siis on `{App-Id}` `{App-Uri-Id}` see sama ja sama.
5. Lisateavet leiate teemast [PROBLEEMID SAML-i-põhisesse ühekordse sisselogimisega konfigureeritud rakendustesse sisselogimisel.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**Rakenduste kohandamine**

- [Lisage ettevõtte](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) Azure Active Directory sisselogimislehele margitoodete lisamine . Kasutage oma asutuse logo ja kohandatud värviskeeme, et pakkuda oma Azure Active Directory (Azure AD) sisselogimislehtedele ühtse ilme.
- [Lisage kohandatud domeeninimi portaali Azure Active Directory –](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) igal uuel Azure AD rentnikul on algne domeeninimi. Algset domeeninime ei saa muuta ega kustutada, kuid saate lisada oma asutuse nimesid. Kohandatud domeeninimede lisamine aitab teil luua kasutajatele tuttavaid kasutajanimesid.
