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
ms.openlocfilehash: 62f667cccd0761e081b3f651709fadfec12500e76fd8e30b8649a28e99001e4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966033"
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

1. Lühiülevaate: saml-põhise ühekordse sisselogimise (SSO) häälestamine rakenduse jaoks [oma Azure Active Directory (Azure AD) rentnikus.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)
2. Lisateavet saml-põhise ühekordse sisselogimise suvandi kohta leiate teemast [SAML-i-põhise ühekordse sisselogimise mõistmine.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)
3. Lisateavet saml 2.0 autentimistaotluste ja vastuste kohta, mida Azure Active Directory (Azure AD) toetab ühekordse Sign-On (SSO) jaoks, leiate teemast Sign-On [SAML-i protokoll.](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
4. Teavet selle kohta, kuidas luua ja konfigureerida microsoft Graph API-ga rakenduses Azure Active Directory (Azure AD) oma rakenduse jaoks SAML-i-põhise ühekordse sisselogimise (SSO) konfigureerimine, leiate teemast [SAML-i-põhise](https://docs.microsoft.com/graph/application-saml-sso-configure-api)ühekordse sisselogimise konfigureerimine rakenduse jaoks Microsoft Graph API abil.
5. Teavet selle kohta, kuidas Azure AD KASUTAB SAML-protokolli, leiate teemast [Microsofti identimisplatvorm KASUTAB SAML-protokolli.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)

**Märkide ja nõuete konfigureerimine**

1. [Kuidas: kohandada SAML-i loas ettevõtterakenduste jaoks välja antud nõudeid.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)
2. PowerShelli abil nõuete konfigureerimise kohta leiate teavet teemast Kuidas: rentnikus konkreetse rakenduse märkides välja heitnud nõuete [kohandamine (eelvaade).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
3. Lisateavet valikuliste nõuete konfigureerimise kohta leiate teemast [Kuidas: rakendusele valikuliste nõuete esitamine.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
4. Teavet selle kohta, kuidas kasutada kataloogiskeemilaiendi atribuute kasutajaandmete saatmiseks loataotlustes rakendustesse, leiate teemast [Kataloogiskeemilaiendi atribuutide kasutamine nõuetes.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions)
5. Teavet loa kasutusaja konfigureerimise kohta leiate teemast Märkide konfigureerimine Microsofti identimisplatvorm [(eelvaade).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. [Kasutusaja poliitikate konfigureerimine (eelvaade)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) – selles artiklis läbime ühise poliitikastsenaariumi, mis aitab teil kehtestada uusi reegleid loa eluea kohta. Näites saate teada, kuidas luua poliitika, mis nõuab kasutajatelt teie veebirakenduses sagedamini autentimist.

**SSO konfiguratsiooni tõrkeotsing**

- Korduma kippuvad küsimused sujuva Azure Active Directory ühtse Sign-On kohta leiate [teemast Azure Active Directory Sujuv ühekordne sisselogimine: korduma kippuvad küsimused.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq)
- Levinud probleemide tõrkeotsingu kohta Azure Active Directory (Azure AD) Sign-On (Sujuv SSO) leiate teemast [Azure Active Directory sujuv ühekordne sisselogimine.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)
