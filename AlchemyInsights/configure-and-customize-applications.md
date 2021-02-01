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
ms.openlocfilehash: 30127beda85dd9824f7e3a7a4744d109e7ea874b
ms.sourcegitcommit: aeb15e206865f61ff61a1e55c407e34eaa89b6d1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063617"
---
# <a name="configure-and-customize-applications"></a>Rakenduste konfigureerimine ja kohandamine

**Rakenduste konfigureerimine**

1. [Kiirjuhend: rakenduse atribuutide konfigureerimine Azure Active Directory (AZURE ad) rentniku jaoks](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) kuvab rakenduse atribuutide konfigureerimine.
2. Rakenduste integreerimiseks Azure Active Directoryga oleme koostanud [õpikute kogumi](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) , mis juhatavad teid läbi konfiguratsiooni.
3. [Rakenduse puhverserveri rakenduse konfigureerimine](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) aitab teil aru saada, kuidas konfigureerida rakenduse puhverserveri rakendust Azure AD-s, et teie kohapealseid rakendusi pilve paljastada.
4. [Laadige alla PingAccess ja konfigureerige oma rakendus](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application): JÄRGIGE *Azure AD PingAccess konfigureerimise juhiseid, et kaitsta* Microsoft Azure AD Application puhverserveri kaudu avaldatud rakendusi ping identiteedi veebisaidil ja laadida alla PingAccess uusim versioon.

**Valesti konfigureeritud rakenduse (AADSTS650056) tõrked**

1. Veenduge, et pääsete rakendusele juurde rakenduse omaniku antud sisselogimise aadressilt. Muus tähenduses logige rakendusse sisse selle tavalise protsessi kaudu. Enamikel juhtudel saab see automaatselt lahendada loomulikult. Kui seda ei juhtu, saab see postitus aidata selle tõrkeotsingul ja lahendamisel.
2. **Kui teie ettevõte omab rakendust** (mis tähendab, et rakenduse registreerimine on teie asutuses):
    - Vähemalt soovitame `User.Read` `openid` lisada **Microsoft Graphi** või delegeeritud õigused.
    - Veenduge, et rakendus ja kõik selle load on nõus. Seda saab kontrollida, kui otsite API-i **õigustes** rakenduse registreerimise veeru **olekut** .
    - Mõnel juhul võib rakendus olla kolmanda osapoole konto, kuid see võib olla teie asutuses registreeritud. Kinnitage, kas see rakendus on teie rakenduse registreerimistes (mitte Enterprise Applications) loetletud.
    - Kui jätkate selle tõrketeate kuvamist. Seejärel peate võib-olla koostama **juhises 4** kirjeldatud nõusoleku URL-i.
3. **Kui teie asutus pole rakenduse omanik ja kasutate seda kolmanda osapoole rakendusena, tehke** järgmist.
    - Kui olete globaalne/ettevõtte administraator, peaksite nägema nõusoleku Kuva. Veenduge, et märgite ruudu **"nõusolek organisatsiooni nimel"**.
    - Kui te ei näe nõusoleku Kuva, kustutage ettevõtte rakendus ja proovige uuesti.
    - Kui jätkate selle tõrketeate kuvamist. Seejärel peate võib-olla koostama **juhises 4** kirjeldatud nõusoleku URL-i.
4. Saate **käsitsi luua kasutatava nõusoleku URL-i**: kui rakendus on mõeldud juurdepääsuks kindlale ressursile, ei pruugi teil olla võimalik kasutada Azure ' i portaalis nõusoleku nuppe, peate käsitsi looma oma nõusoleku URL-i ja kasutama seda.
    - Peate hankima `{App-Id}` `{App-Uri-Id}` rakenduse omaniku ja selle rakenduse omanikult. `{Tenant-Id}` on teie rentniku identifikaator. See on kas `yourdomain.onmicrosoft.com` või teie kataloogi ID.
    - Kui rakendus kasutab ressurssi ise, siis on see `{App-Id}` `{App-Uri-Id}` sama.
5. Lisateavet leiate teemast Sisselogimine [SAML-põhisesse ühekordse sisselogimise konfigureeritud rakendusse](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application).

**Rakenduste kohandamine**

- [Oma ettevõtte Azure Active Directory ' i sisselogimise lehe lisamine](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) – saate kasutada oma asutuse logo ja kohandatud värviskeeme, et anda oma Azure Active Directory (Azure AD) sisselogimise lehtedele järjepidev ilme ja tunne.
- [Kohandatud domeeninime lisamine Azure Active Directory portaali abil](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) – iga uus Azure AD rentnik sisaldab algset domeeninime. Te ei saa algset domeeninime muuta või kustutada, kuid saate lisada oma asutuse nimed. Kohandatud domeeninimede lisamine aitab luua kasutajate tuttavaid kasutajanimesid.
