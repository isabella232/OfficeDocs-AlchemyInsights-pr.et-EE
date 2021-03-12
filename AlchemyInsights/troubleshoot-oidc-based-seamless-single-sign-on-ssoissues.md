---
title: OIDC-põhiste tõrgeteta ühekordse sisselogimise (SSO) probleemide tõrkeotsing
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
ms.openlocfilehash: e4ddde6176d9ab021b93e23b3cb363e10b1c1048
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743974"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>OIDC-põhiste tõrgeteta ühekordse sisselogimise (SSO) probleemide tõrkeotsing

- Lisateavet Azure ' i rentniku OIDC-põhise rakenduse lisamise kohta leiate teemast [Kiirjuhend: OIDC-põhise ühekordse sisselogimise (SSO) häälestamine Azure Active Directory (AZURE ad) rentniku jaoks mõeldud rakenduse jaoks](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso).
- Lisateavet rakenduste kohta, mis kasutavad funktsiooni OpenID Connect Standard ühekordse sisselogimise rakendamiseks, leiate teemast [OIDC põhinev Ühekordne sisselogimine](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on).
- Lisateabe saamiseks juhuks, kui soovite oma koodi kirjutada otse HTTP päringute saatmisel või käsitlemisel või kasutada mõne muu tootja avatud lähtekoodiga teeki, mitte kasutada ühte meie avatud lähtekoodiga teekidest, lugege teemat [oauthi 2,0 ja OpenID Connecti Microsoft Identity Platform ' i protokollid](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols).

**Protokollid**

1. [Microsoft Identity Platform ja kaudne Grant Flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) – kaudse toetuse iseloomulikud tunnused on see, et/Token lõpp-punkti asemel tagastatakse märked (ID-või juurdepääsuluba) otse/authorize lõpp-punktist. Seda kasutatakse sageli loa koodi voo osana, mille nimeks on **"hübriid-voog" – ID-märgi hankimine/authorize taotlusele koos loa koodiga**. Selles artiklis kirjeldatakse, kuidas rakendusest Azure AD saadud märkide taotlemiseks otse rakenduse protokolli vastu.
2. [Microsoft Identity Platform ja oauthi 2,0 autoriseerimise koodi voog](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) – OAuthi 2,0 luba saab kasutada rakendustes, mis on seadmesse installitud, et pääseda juurde kaitstud ressurssidele (nt veebirakendusliidestele). OAuthi 2,0 Microsofti identiteedi platvormi rakendamise abil saate **lisada sisselogimist ja API juurdepääsu oma mobiil-ja töölaua rakendustele**. Selles artiklis kirjeldatakse, kuidas programmeerida rakenduse protokolli vastu mis tahes keeles.
3. [Microsofti identiteedi platvormi ja OpenID Connecti protokoll](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) – kui kasutate Microsofti identiteedi platvormi rakendamist OpenID Connecti kaudu, saate oma rakendustele lisada SISSELOGIMISE ja API-juurdepääsu. Selles artiklis kirjeldatakse, kuidas teha seda keelest sõltumatult ja kuidas **saata ja vastu võtta http-sõnumeid ilma ühegi Microsofti avatud lähtekoodiga teegita**.
4. [Microsoft Identity Platform ja oauthi 2,0 Client mandaatide voog](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) – saate kasutada OAuthi 2,0, mis on määratud RFC 6749 (mõnikord ka **kahe jalaga OAuthi**), et pääseda juurde veebi kaudu hallatavatele ressurssidele rakenduse identiteedi abil. Seda tüüpi toetust kasutatakse tavaliselt server-to-serveriga suhtlemiseks, mis peavad taustal töötama, kui kasutaja ei saa seda kohe teha. Seda tüüpi rakendusi nimetatakse sageli nii **deemonite** kui ka **teenuse kontode** jaoks. Selles artiklis kirjeldatakse, kuidas programmeerida programm otse teie rakenduse protokolli vastu.
