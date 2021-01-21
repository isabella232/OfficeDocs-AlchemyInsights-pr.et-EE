---
title: Märkidega seotud probleemid
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916846"
---
# <a name="issues-with-tokens"></a>Märkidega seotud probleemid

Märkidega seotud probleemide haldamiseks saate teha järgmisi toiminguid.

1. Saate määrata Microsoft Identity Platformi poolt välja antud Accessi, ID või SAML kestuse. Saate määrata märkide eluea kõigi oma asutuse rakenduste jaoks, mitme rentniku (mitme organisatsiooni) rakenduse jaoks või ettevõtte teatud teenuse põhiosa jaoks. Lisateavet leiate teemast [Konfigureeritav turbelubade eluiga Microsoft Identity Platform ' is (eelvaade)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. Accessi märgid võimaldavad klientidel turvaliselt kasutada kaitstud veebiapi-sid, mida veebirakendusliidesed kasutavad autentimise ja autoriseerimise teostamiseks. OAuthi-i määratluse korral on Accessi märkideks läbipaistmatud stringid, mis ei ole määratud vormingus – mõned identiteedi pakkujad (sisepagulaste reintegreerimine) kasutavad GUID-e, teised kasutavad krüptitud blob-e. Microsoft Identity Platform kasutab mitmesuguseid Accessi turbelubade vorminguid, olenevalt sellest, millist API-d aktsepteerib luba. Lisateavet selle kohta, kuidas teie API saab valideerida ja kasutada Accessi tõendites olevaid argumente, leiate teemast [Microsofti identiteedi platvormi juurdepääsuluba](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint).
3. Microsofti autentimise teek (MSAL) toetab mitmeid autentimise voogusid eri rakenduse stsenaariumite jaoks. Lisateavet leiate teemast [autentimise vood](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes).
4. OAuthi 2,0 tegevusluba saab kasutada rakendustes, mis on seadmesse installitud, et pääseda juurde kaitstud ressurssidele (nt veebirakendusliidestele). OAuthi 2,0 Microsofti identiteedi platvormi rakendamise abil saate lisada sisselogimise ja API juurdepääsu oma mobiil-ja töölaua rakendustele. Lisateavet leiate teemast [Microsofti identiteedi platvorm ja oauthi 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) , kuidas programmeerida rakenduses mis tahes keeles otse protokollile vastavat protokolli.
5. OpenID Connect (OIDC) on OAuthi 2,0 jaoks loodud autentimise protokoll, mida saate kasutada rakenduse kasutaja turvaliseks sisselogimiseks. Kui kasutate Microsofti identiteedi platvormi lõpp-punkti rakendamist OpenID Connecti kaudu, saate oma rakendustele lisada sisselogimise ja API-juurdepääsu. [Microsofti identiteedi platvormi ja OpenID Connecti protokoll](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) näitab, kuidas seda keelest sõltumatult teha ja kuidas saata ja vastu võtta http-sõnumeid ilma ühegi Microsofti avatud lähtekoodiga teegi kasutamata.
    - UserInfo lõpp-punkt on osa OIDC standardist, mille eesmärk on tagastada nõuded autenditud kasutaja kohta. Lisateavet leiate teemast [Microsofti identiteedi platvormi UserInfo lõpp-punkt](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead).
    - Veebiväljaandele veebiväljaandele [helistamine AZURE ad ja OpenID Connecti proovi abil](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) näitab, kuidas luua MVC veebirakendus, mis kasutab Azure AD sisselogimiseks OpenID Connecti protokolli abil, ja seejärel helistage sisse logitud kasutaja identiteedi alusel OAuthi 2,0 kaudu saadud märkide abil. See valim kasutab OpenID Connect ASP .net OWIN vahevara ja ADAL .net.
6. [Rakenduse konfigureerimine VEEBIrakendusliidese kuvamiseks](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) – selles Kiirjuhend registreerite veebirakendusliidese Microsofti identiteedi platvormiga ja saate selle lisada klientrakenduse kaudu, lisades näite ulatuse. Kui registreerid oma veebirakendusliidese ja jätad selle läbi ulatuste, saate oma ressurssidele anda õigusi kasutavatele juurdepääsu oma ressurssidele autoriseeritud kasutajatele ja klientrakendustele, mis pääsevad teie API-sse.
7. Azure Active Directory B2C (Azure AD B2C) ressursi omanik parooli mandaat (ROPC) voog on OAuthi Standard Authentication Flow. Selle voo korral on rakendus, mida nimetatakse ka vastavaks osapooleks, Exchange ' i märkide jaoks kehtivaid mandaate. Mandaat sisaldab kasutajanime ja parooli. Tagastatav märk on ID-märk, juurdepääsuluba ja värskendav märk. Lisateavet leiate teemast [Ressursi omaniku parooli mandaadi voo häälestamine Azure Active DIRECTORY B2C](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow). 

