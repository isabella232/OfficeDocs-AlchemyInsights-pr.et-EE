---
title: OIDC-põhise sujuva ühekordse sisselogimise (SSO) probleemide tõrkeotsing
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
- "9375"
ms.openlocfilehash: 5880ee37a2fcc98b34231cc9960fb3f87fa184b07bd81ccd37d0ea5a78170af0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105769"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>OIDC-põhise sujuva ühekordse sisselogimise (SSO) probleemide tõrkeotsing

- Lisateavet OIDC-põhise rakenduse azure'i rentnikule lisamise kohta leiate teemast [Quickstart: OIDC-põhise ühekordse sisselogimise (SSO) häälestamine rakenduse jaoks oma Azure Active Directory (Azure AD) rentnikus.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)
- Lisateavet rakenduste kohta, mis kasutavad OpenID-Ühendus standardit ühekordse sisselogimise juurutamiseks, leiate teemast [OIDC-põhise ühekordse sisselogimise mõistmine.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on)
- Lisateavet juhuks, kui otsustate kirjutada oma koodi otse HTTP-päringute saatmise ja käitlemisega või kasutada kolmanda osapoole avatud lähtekoodiga teeki, mitte meie avatud lähtekoodiga teeke, lugege [teemat OAuth 2.0 ja OpenID Ühendus protokollid Microsofti identimisplatvorm](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols).

**Protokollid**

1. [Microsofti identimisplatvorm](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) ja kaudne andmine – kaudse toetuse määratlev omadus on see, et märgid (ID-märgid või juurdepääsutõend) tagastatakse otse lõpp-punktist /authorize, mitte /token lõpp-punktist. Seda kasutatakse sageli autoriseerimiskoodi voo osana, mida nimetatakse hübriidvooks – ID-märgi toomine autoriseerimistaotluses koos **autoriseerimiskoodiga.** Selles artiklis kirjeldatakse, kuidas otse rakenduse protokolli vastu programmeerida, et taotleda Azure AD-lt tõendeid.
2. [Microsofti identimisplatvorm ja OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) autoriseerimiskoodi voog – OAuth 2.0 autoriseerimiskoodi andmist saab kasutada rakendustes, mis on seadmesse installitud, et pääseda juurde kaitstud ressurssidele (nt veebi API-d). Kui kasutate Microsofti identimisplatvorm OAuth 2.0, saate lisada sisse- ja **API-juurdepääsu oma mobiili- ja töölauarakendustele.** Selles artiklis kirjeldatakse, kuidas otse rakenduse protokolli vastu mis tahes keeles programmeerida.
3. [Microsofti identimisplatvorm ja OpenID Ühendus](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) - Kui kasutate Microsofti identimisplatvorm'i OpenID-i Ühendus, saate oma rakendustele lisada sisselogimis- ja API-juurdepääsu. Selles artiklis kirjeldatakse, kuidas seda teha sõltumata keelest ja kuidas http-sõnumeid saata ja vastu võtta ilma **Microsofti avatud lähtekoodiga teeke kasutamata.**
4. [Microsofti identimisplatvorm ja OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) kliendi identimisteabe voog – saate kasutada OAuth 2.0 kliendi identimisteabe andmist, mis on määratud RFC 6749-s (mõnikord nimetatakse seda kahejalgseks **OAuthiks),** et pääseda juurde veebimajutuse ressurssidele, kasutades rakenduse identiteeti. Seda tüüpi toetust kasutatakse tavaliselt serverist serverisse suhtlemiseks, mis peab taustal käivituma ilma kohese suhtluseta kasutajaga. Seda tüüpi rakendusi nimetatakse sageli **deemoniks või** **teenusekontoks.** Selles artiklis kirjeldatakse, kuidas otse rakenduse protokolli vastu programmeerida.
