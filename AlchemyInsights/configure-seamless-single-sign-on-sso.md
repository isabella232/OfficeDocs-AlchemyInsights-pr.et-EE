---
title: Sujuva ühekordse sisselogimise konfigureerimine (SSO)
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
- "9004344"
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: bd3873c2db1b8d548f81d531a8bf5747130fe761
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402263"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Sujuva ühekordse sisselogimise konfigureerimine (SSO)

**Rakenduste konfigureerimine**

1. Peaksite väärtused saama rakenduse tarnijalt. Väljade väärtuse ekstraktimiseks saate väärtused käsitsi sisestada või metaandmete faili üles laadida.
2. Paljud rakendused on azure AD-ga tööks juba eel konfigureeritud. Need rakendused on loetletud rakenduste galeriis, mida saate sirvida, kui lisate rakenduse Azure AD rentnikule. Kiirsari [juhatab](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) teid läbi protsessi.
3. Mittegaleriirakenduse loomiseks klõpsake nuppu **+ Loo** oma rakendus ja andke oma rakendusele nimi.
    - Vaikimisi valige galeriist Integreeri kõik muud rakendused, mida te ei leia **ja** mis on mittegaleriirakenduste jaoks õige valik.
    - Kui olete **pärast** rakenduse nime panemist vajutanud nuppu Loo, luuakse uus mittegalerii Enterprise'i rakendus.
    - Seejärel võite jaotises  Halda seda rakendust  liikuda jaotisse Ühekordne sisselogimine ja saate vaadata erinevaid tehnikaid selle rakendamiseks oma keskkonnas.

**Kindla rakenduse sujuva SSO konfigureerimine**

Galeriis kuvatavate rakenduste kohta leiate üksikasjalikud üksikasjalikud juhised. Juhistele juurdepääsemiseks saate sirvida saaS-i rakenduse konfigureerimise õppevideotes kõigi rakenduse [konfigureerimise õppevideote loendit.](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)

**SAML-põhise SSO konfigureerimine**

1. [Lühiülevaate: rakenduse JAOKS SAML-i-põhise ühekordse sisselogimise (SSO) häälestamine Azure Active Directory (Azure AD) rentnikus.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)
2. Lisateavet saml-põhise ühekordse sisselogimise suvandi kohta leiate teemast [SAML-i-põhise ühekordse sisselogimise mõistmine.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)
3. Lisateavet saml 2.0 autentimistaotluste ja vastuste kohta, mida Azure Active Directory (Azure AD) toetab ühekordse Sign-On (SSO) jaoks, leiate teemast Sign-On [SAML-i protokoll.](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
4. Teavet selle kohta, kuidas microsoft Graph API-ga Azure Active Directorys (Azure AD) luua ja konfigureerida oma rakenduse jaoks SAML-i-põhine ühekordne sisselogimine (SSO), leiate teemast [SAML-i-põhise](https://docs.microsoft.com/graph/application-saml-sso-configure-api)ühekordse sisselogimise konfigureerimine rakenduse jaoks Microsoft Graph API abil.
5. Teavet selle kohta, kuidas Azure AD KASUTAB SAML-protokolli, leiate teemast [Microsofti identiteediplatvormi kasutamine SAML-protokollis.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)

**Märkide ja nõuete konfigureerimine**

1. [Kuidas: kohandada SAML-i loas ettevõtterakenduste jaoks välja antud nõudeid.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)
2. PowerShelli abil nõuete konfigureerimise kohta leiate teavet teemast Kuidas: rentnikus konkreetse rakenduse märkides välja heitnud nõuete [kohandamine (eelvaade).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
3. Lisateavet valikuliste nõuete konfigureerimise kohta leiate teemast [Kuidas: rakendusele valikuliste nõuete esitamine.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
4. Teavet selle kohta, kuidas kasutada kataloogiskeemilaiendi atribuute kasutajaandmete saatmiseks loataotlustes rakendustesse, leiate teemast [Kataloogiskeemilaiendi atribuutide kasutamine nõuetes.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions)
5. Teavet selle kohta, kuidas konfigureerida loa eluiga, leiate teemast Microsofti identiteediplatvormi konfigureeritavate märkide [kasutusajad (eelvaade).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. [Kasutusaja poliitikate konfigureerimine (eelvaade)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) – selles artiklis läbime ühise poliitikastsenaariumi, mis aitab teil kehtestada uusi reegleid loa eluea kohta. Näites saate teada, kuidas luua poliitika, mis nõuab kasutajatelt teie veebirakenduses sagedamini autentimist.

**SSO konfiguratsiooni tõrkeotsing**

- Korduma kippuvad küsimused Azure Active Directory sujuva Sign-On (sujuv SSO) kohta leiate teemast Azure Active Directory sujuv ühekordne [sisselogimine: korduma kippuvad küsimused.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq)
- Azure Active Directory (Azure AD) sujuva ühekordse sisselogimisega (Azure AD) seotud levinud probleemide tõrkeotsingu Sign-On kohta leiate teavet teemast [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)sujuva ühekordse sisselogimise tõrkeotsing.
