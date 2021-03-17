---
title: Sujuva ühekordse sisselogimise (SSO) konfigureerimine
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
- "9384"
ms.openlocfilehash: 32790b23547de36cd2864e85ebae67f54ad91707
ms.sourcegitcommit: 309b9f3e6e2ff622f95bb860d337d2c05b7bbe54
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/15/2021
ms.locfileid: "50841458"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Sujuva ühekordse sisselogimise (SSO) konfigureerimine

**Rakenduste konfigureerimine**

1. Peaksite hankima rakenduse tarnija väärtused. Väljade väärtuse ekstraktimiseks saate väärtused käsitsi sisestada või metaandmete faili üles laadida.
2. Paljud rakendused on Azure AD-ga töötamiseks juba eelnevalt konfigureeritud. Need rakendused on loetletud rakenduste galeriis, mida saate sirvida, kui lisate Azure AD rentniku jaoks rakenduse. [Kiirjuhend sari](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) juhendab teid protsessi käigus.
3. Mitte-Galerii rakenduse loomiseks saate klõpsata nuppu **+ luua oma rakenduse** ja anda oma rakendusele nime.
    - Vaikimisi valitakse **muude rakenduste integreerimine galeriist** , mis ei ole Galerii rakenduste jaoks õige valik.
    - Kui pärast rakenduse nime sisestamist on pärast käivitamist **loodud** uus rakendus, loob see uue mitte-Galerii Enterprise ' i rakenduse.
    - Seejärel võite liikuda **ühe sisselogimise** all selle rakenduse **haldamisel** ja teil on võimalik näha erinevaid tehnikaid selle rakendamiseks teie keskkonnas.

**Kindla rakenduse jaoks õmblusteta SSO konfigureerimine**

Galerii rakenduste jaoks leiate üksikasjalikud, üksikasjalikud juhised. Toimingute juurde pääsemiseks saate sirvida kõigi rakenduse konfiguratsiooni õpetuste loendit aadressil [Saas app Configuration Tutorials](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list).

**SAML-põhise SSO konfigureerimine**

1. [Kiirjuhend: SAML-põhise ühekordse sisselogimise (SSO) häälestamine Azure Active Directory (AZURE ad) rentniku jaoks mõeldud rakenduse jaoks](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso).
2. Lisateavet SAML-põhise suvandi ühekordse sisselogimise kohta leiate teemast [SAML-põhise ühekordse sisselogimise](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)võimalus.
3. Lisateavet SAML 2,0 autentimise taotluste ja vastuste kohta, mille Azure Active Directory (Azure AD) toetab ühekordse Sign-On (SSO) jaoks, leiate teemast [ühtse Sign-On SAML protokoll](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol).
4. Lisateavet selle kohta, kuidas luua ja konfigureerida rakenduse Azure Active Directory (Azure AD) SAML põhinev ühekordse sisselogimise (SSO) rakendus Microsoft Graph API abil, lugege teemast [rakenduse SAML-põhise ühekordse sisselogimise konfigureerimine Microsoft GRAPHI API abil](https://docs.microsoft.com/graph/application-saml-sso-configure-api).
5. Lisateavet selle kohta, kuidas Azure AD SAML protokolli kasutab, leiate artiklist [Kuidas Microsoft Identity Platform kasutab SAML protokolli](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference).

**Märkide ja nõuete konfigureerimine**

1. [Juhised: SAML-i turbelubade jaoks välja antud nõuete kohandamine](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).
2. Lisateavet PowerShelli abil nõuete konfigureerimise kohta leiate teemast [Kuidas: rentniku teatud rakenduse märkidest eralduvate nõuete kohandamine (eelvaade)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
3. Lisateavet valikuliste nõuete konfigureerimise kohta leiate teemast [Kuidas: oma rakendusele valikuliste nõuete esitamine](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
4. Lisateavet selle kohta, kuidas kasutada kataloogi skeemi laiendi atribuute taotluste saatmiseks turbelubade taotlustes, leiate teemast [Directory skeemi laiendi atribuutide kasutamine nõuetes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. Lisateavet märkide eluajal konfigureerimise kohta leiate teemast [Konfigureeritav turbelubade eluiga Microsoft Identity Platform ' is (eelvaade)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
6. [Märkide eluaegsete poliitikate konfigureerimine (eelvaade)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) – selles artiklis me käime ühise poliitika stsenaariumis, mis aitab teil kehtestada uusi reegleid turbelubade eluajal. Näites saate teada, kuidas luua poliitika, mis nõuab kasutajatelt teie veebirakenduses sagedamini autentimist.

**SSO konfiguratsiooni tõrkeotsing**

- Korduma kippuvad küsimused Azure Active Directory õmblusteta ühekordse Sign-On (õmblusteta SSO) kohta leiate teemast [Azure Active Directory sujuv Ühekordne sisselogimine: korduma kippuvad küsimused](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).
- Azure Active Directory (Azure AD) õmblusteta ühekordse Sign-On (õmblusteta SSO) levinumate probleemide tõrkeotsingu kohta leiate teavet teemast [Azure Active Directory õmblusteta ühekordse sisselogimise tõrkeotsing](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso).
