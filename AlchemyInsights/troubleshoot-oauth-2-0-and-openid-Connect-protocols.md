---
title: OAuthi 2,0 ja OpenID Connecti protokollide tõrkeotsing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: d2f14d4d16bea890b564cdb9bd9ac3875c28d115
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035596"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>OAuthi 2,0 ja OpenID Connecti protokollide tõrkeotsing

OAuthi 2,0 ja OpenID Connecti probleemide lahendamiseks tehke järgmist soovitatud toiminguid.

Lugege järgmisi artikleid, mis on seotud OAuthi 2,0 ja OpenID ühendamise protokollide konfigureerimise ja tõrkeotsinguga.

- [Microsoft Identity Platform ja oauthi 2,0 autoriseerimise kood Flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) -selles artiklis kirjeldatakse, kuidas programmeerida otse rakenduses **kood Grant (PKCE)** , kasutades mis tahes keelt.
- [Microsoft Identity Platform ja oauthi 2,0 Client mandaatide voog](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) – selles artiklis kirjeldatakse, kuidas programmeerida programm otse rakenduse **Client mandaatide voogude** vastu.
- [Microsoft Identity Platform ja oauthi 2,0 ressursi omaniku parooli mandaat](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) – selles artiklis kirjeldatakse, kuidas programmeerida otse rakenduse **ROPC** .
    - Microsofti identiteedi platvorm toetab ainult ROPC Azure AD rentnike jaoks, mitte isiklike kontode jaoks. See tähendab, et peate kasutama rentniku-spetsiifilist lõpp-punkti **( https://login.microsoftonline.com/{TenantId_or_Name})** või **organisatsioonide** lõpp-punkti).
    - Azure AD rentniku kutsutud isiklikud kontod ei saa ROPC kasutada.
    - Kontod, millel pole paroole, ei saa ROPC kaudu sisse logida. Selle stsenaariumi korral soovitame kasutada rakenduse asemel erinevat voogu.
    - Kui kasutajad peavad rakenduse sisse logimiseks kasutama [mitme teguri autentimist (MFA)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) , siis need blokeeritakse.
    - ROPC ei toeta hübriid- [identiteedi Föderatsiooni](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) stsenaariumid (nt Azure AD ja ADFS, mida kasutatakse kohapealsete kontode autentimiseks). Kui kasutajad on kogu saidil ümber suunatud kohapealsele identiteedi pakkujale, ei saa Azure AD selle identiteedi pakkuja kasutajanime ja parooli testida. ROPC kaudu toetatakse [edasi-tagasiautentimist](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) .
    - Hübriid-identiteedi Föderatsiooni stsenaariumi erandiks on järgmine: kodu Realm Discovery poliitika, mille **AllowCloudPasswordValidation** väärtuseks on seatud **True** , võimaldab ROPC voo töötamiseks väliskasutajatele, kui asutusesisene parool sünkroonitakse pilvega. Lisateavet leiate teemast [Väliskasutajate jaoks mõeldud ROPC autentimise lubamine Legacy-rakenduste jaoks](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) 
- [Microsoft Identity Platform ja oauthi 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) (-nimel) – selles artiklis kirjeldatakse, kuidas programmeerida programm otse teie rakenduse **nimel (OBO)** .
- [Microsofti identiteedi platvormi ja OpenID Connecti protokoll](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) – selles artiklis kirjeldatakse, kuidas rakendada OpenID Connecti protokoll keelest sõltumatu, ning kirjeldatakse, kuidas saata ja vastu võtta http-sõnumeid ilma ühegi Microsofti avatud lähtekoodiga teegita.

**Juurdepääsuluba**

[Microsoft Identity Platform Accessi märked](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – saate teada, kuidas teie API saab kinnitada ja kasutada Accessi loaga esitatud nõudeid. Kõik selle artikli dokumendid, välja arvatud juhul, kui need on märgitud, rakenduvad ainult registreeritud API-de jaoks väljaantud märkide korral. Seda ei kohaldata Microsofti omanduses olevate API-de jaoks välja antud märkide suhtes, samuti ei saa neid märke kasutada selleks, et valideerida, kuidas Microsoft Identity Platform teie loodud API jaoks lube väljastab.

**Rakenduse konfigureerimine**

[SUUNA URI (vasta URL) piirangud ja piirangud](https://docs.microsoft.com/azure/active-directory/develop/reply-url) – saate teada, kuidas konfigureerida oma ümbersuunamise URI (vasta URL). Ümbersuunamise URI või vastuse URL on koht, kus autoriseerimise server saadab kasutaja, kui rakendus on edukalt autoriseeritud ja andis loa koodi või juurdepääsuluba. Autoriseerimise server saadab koodi või tõendi ümbersuunamise URI-sse; Seega on oluline, et registreerid rakenduse registreerimisprotsessi osana õige asukoha.

**Rakenduse ettevalmistamine**

[Õpetus: SCIM lõpp-punkti ettevalmistamine ja kavandamine](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) – selles artiklis kirjeldatakse, kuidas luua SCIM lõpp-punkti ja integreerida AAD ettevalmistamise teenusega.


