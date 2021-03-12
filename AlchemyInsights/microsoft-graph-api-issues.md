---
title: Microsoft Graphi API probleemid
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
- "9004345"
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/29/2021
ms.locfileid: "50713701"
---
# <a name="microsoft-graph-api-issues"></a>Microsoft Graphi API probleemid

See teema võib kehtida ka siis, kui arendajad kasutavad endiselt Azure AD Graph API-d. Siiski on **tungivalt** soovitatav kasutada Microsoft Graphi kõigi kataloogide, identiteedi ja Accessi halduse stsenaariumite jaoks.

**Autentimise või autoriseerimisega seotud probleemid**

- Kui teie rakendus ei saa Microsofti graafikule helistamiseks **märke hankida** , valige **probleem** , kui soovite selle teema kohta täpsemat abi ja tuge hankida Microsoft Graphi kategooria kaudu.
- Kui rakenduses Microsoft Graph helistamisel kuvatakse rakenduse **401 või 403 lubamise tõrked** , **Valige selle teema** kohta täpsema abi ja toe hankimiseks Microsoft Graph API kategooria.

**Soovin kasutada rakendust Microsoft Graph, kuid pole kindel, kust alustada**

- [Microsoft Graphi ülevaade](https://docs.microsoft.com/graph/overview)
- [Microsoft Graphi identiteedi ja Accessi halduse ülevaade](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Microsoft Graphi rakenduste loomise alustamine](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – Microsoft Graphi API-de testimine rentniku või demo rentniku jaoks

**Soovin kasutada rakendust Microsoft Graph, kuid see toetab ka v 1.0 kataloogi API-sid, mida vajan?**

Microsoft Graph on soovitatav API kataloogis, identiteedis ja Accessi halduses. Siiski on võimalik, et Azure AD Graphis ja Microsoft Graphis on veel mõned lüngad. Vaadake üle järgmised artiklid, kus on esile tõstetud kõige ajakohased erinevused teie valitud abistamiseks.

- [Ressursi tüübi erinevused Azure AD Graphis ja Microsoft Graphis](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Azure AD Graphi ja Microsoft Graphi atribuutide erinevused](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Azure AD ja Microsoft Graphi erinevuste meetod](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**API, mida ma helistan, ei tööta – kus saab teha veel teste?**

**Microsoft Graph Explorer** – testige Microsoft Graphi API-sid rentniku või demo rentniku jaoks ja vaadake ka Microsoft Graphi Exploreri **päringute päringuid** .

**Minu rakendus on liiga aeglane ja seda saab ka ahendada. Milliseid täiustusi saab teha?**

Olenevalt teie stsenaariumist on teie käsutuses mitmeid võimalusi, mis aitavad teil oma rakendust rohkem teha, ja mõnel juhul on teenusel vähem altid (kui teete liiga palju kõnesid).

- [Microsoft Graphi head tavad](https://docs.microsoft.com/graph/best-practices-concept)
- [Partiide taotlemine](https://docs.microsoft.com/graph/json-batching)
- [Muutuste jälitus Delta päringu kaudu](https://docs.microsoft.com/graph/delta-query-overview)
- [Muudatustest teavitamine webhooks kaudu](https://docs.microsoft.com/graph/webhooks)
- [Ahendamise juhised](https://docs.microsoft.com/graph/throttling)

**Kust leida lisateavet tõrgete ja teadaolevate probleemide kohta?**

- [Microsoft Graphi tõrgetele reageerimise teave](https://docs.microsoft.com/graph/errors)
- [Microsoft Graphi teadaolevad probleemid](https://docs.microsoft.com/graph/known-issues)

**Kus saab vaadata teenuse kättesaadavuse ja ühenduvuse olekut?**

Teenuste kättesaadavus ja Ühenduvus, millele pääseb juurde Microsoft Graphi kaudu, võib mõjutada Microsoft Graphi üldist kättesaadavust ja jõudlust.

- Azure Active Directory teenuse tervist kontrollitakse [Azure ' i oleku lehel](https://azure.microsoft.com/status/)loetletud **turbe + identiteedi** teenuste olekut.
- Office ' i teenuste jaoks, mis aitavad kaasa Microsoft Graphi, kontrollige [Office ' i teenuse tervise armatuurlaual](https://portal.office.com/adminportal/home#/servicehealth)loetletud teenuste olekut.

Microsoft Graphi loa tõrked võivad olla tingitud mitmest erinevast probleemist, millest enamik tekitab 401 või 403 tõrke. Näiteks võib järgmine tõrketeade olla järgmine:

- valed [pääsutõendi hankimisvood](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- kehvasti konfigureeritud [lubade ulatused](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- puuduv [nõusolek](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

**_Azure Active Directory autentimisteegi (ADAL) ja Azure AD Graphi API (AAD Graphi) tootetoe lõpp_* _

_ * Alates 30 juuni, 2020 * *, me ei lisa enam uusi funktsioone ADAL ja Azure AD Graph. Pakume endiselt tehnilist tuge ja turbevärskendusi, ent mitte enam funktsioonivärskendusi.

**Alates 30 juuni 2022**, lõpetame ADAL ja Azure AD Graphi toe ning ei paku enam tehnilist tuge ega turvavärskendusi.

Rakendused, mis kasutavad ADAL olemasolevatel OPERATSIOONISÜSTEEMI versioonidel, jätkavad tööd ka pärast seda, kuid ei *saa tehnilist tuge ega turvavärskendusi*.

Azure AD Graphi rakendused ei pruugi pärast selle aja möödumist enam saada vastuseid Azure AD Graphi lõpp-punktist.

**ADAL migreerimine**

Soovitame võtta kasutusele [Microsofti autentimisteegi (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), mis sisaldab uusimaid funktsioone ja turbevärskendusi.

Kui kasutate Microsoft apps ' i, saate teada, et Microsoft on oma rakenduste migreerimise protsessis MSAL lõpptähtajaks, tagades, et nad saavad kasu MSAL pidevast turbest ja funktsioonide täiustustest.

1. [Lugege ADAL-i KKK-d.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Lugege lisateavet rakenduste platvormipõhise migreerimise kohta.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Kui vajate abi selle mõistmiseks, mida teie rakendused kasutavad ADAL, soovitame teil kõigi rakenduste lähtekoodi üle vaadata ja vajadusel jõuda kõigi tarkvaratoode või rakenduste pakkujatega. Samuti saab Microsofti tugi anda teile nimekirja kõigist neist mitte-Microsofti rakendustest teie rentnikkeskkonnas, mis kasutavad ADAL-i.

**AAD Graphi migreerimine**

Rakendusi, mis kasutavad Azure AD Graphi, järgige meie juhiseid [AZURE ad Graphi rakenduste migreerimiseks Microsoft Graphi](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Meie migreerimise kontroll-loend on hea koht alustamiseks](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Azure‘i rakenduste registreerimisportaalis näete, millised rakendused kasutavad AAD Graphi. Soovitame teil kõigi rakenduste lähtekood läbi vaadata ja kui vaja, võtta ühendust ISV-de või rakendusepakkujatega. Microsofti tugiteenused võivad teile pakkuda ka teie rentniku kõigi AAD Graphide kasutuse loendit.
3. Rakenduses Microsoft Graph andmetele juurdepääsemiseks peab kasutaja või administraator andma sellele loa andmiseks õiged õigused. [Microsoft Graph permissions References](https://docs.microsoft.com/graph/permissions-reference) loetletakse kõigi Microsoft Graphi API-de põhikomplektiga seotud load. See sisaldab ka juhiseid selle kohta, kuidas kasutada lube.
