---
title: Autentimise teekidega seotud probleemid
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
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063605"
---
# <a name="issues-with-authentication-libraries"></a>Autentimise teekidega seotud probleemid

1. [Microsofti identiteedi platvormi autentimise teegid](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) on loetletud Microsoft-toetatud ja ühilduvad kliendi ja vahevarade teegid
2. Microsofti autentimise teek (MSAL) toetab mitmeid [autentimise voogusid](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) eri rakenduse stsenaariumite jaoks.
3. Märkide autentimiseks ja hankimiseks lähtestage oma koodis uus avalik või konfidentsiaalne klientrakendus. Saate määrata mitu seadistusvõimalusi, kui käivitate Microsofti autentimise teegis (MSAL) klientrakenduse rakenduse. Lisateavet leiate teemast [rakenduse konfigureerimise suvandid](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).

**Azure Active Directory autentimise teegi (ADAL) ja Azure AD Graphi API (AAD Graph) toe lõppemine**

**Alates 30 juunist 2020** ei lisa me enam ADAL ja Azure AD Graphi uusi funktsioone. Pakume endiselt tehnilist tuge ja turbevärskendusi, ent mitte enam funktsioonivärskendusi.

**Alates 30 juuni 2022**, lõpetame ADAL ja Azure AD Graphi toe ning ei paku enam tehnilist tuge ega turvavärskendusi.

Rakendused, mis kasutavad ADAL olemasolevatel OPERATSIOONISÜSTEEMI versioonidel, jätkavad tööd ka pärast seda, kuid ei *saa tehnilist tuge ega turvavärskendusi*.

Azure AD Graphi rakendused ei pruugi pärast selle aja möödumist enam saada vastuseid Azure AD Graphi lõpp-punktist.

**ADAL migreerimine**

Soovitame võtta kasutusele [Microsofti autentimisteegi (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), mis sisaldab uusimaid funktsioone ja turbevärskendusi.

Kui kasutate Microsoft apps ' i, saate teada, et Microsoft on oma rakenduste migreerimise protsessis MSAL lõpptähtpäevaks, tagades, et nad saavad kasu MSAL pidevast turbest ja funktsioonide täiustustest.

Lisateavet leiate järgmistest teemadest:

1. [Lugege ADAL-i KKK-d.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Lugege lisateavet rakenduste platvormipõhise migreerimise kohta.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Kui vajate abi selle mõistmiseks, mida teie rakendused kasutavad ADAL, soovitame teil kõigi rakenduste lähtekoodi üle vaadata ja vajadusel jõuda kõigi tarkvaratoode või rakenduste pakkujatega. Samuti saab Microsofti tugi anda teile nimekirja kõigist neist mitte-Microsofti rakendustest teie rentnikkeskkonnas, mis kasutavad ADAL-i.

**AAD Graphi migreerimine**

Rakendusi, mis kasutavad Azure AD Graphi, järgige meie juhiseid [AZURE ad Graphi rakenduste migreerimiseks Microsoft Graphi](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Meie migreerimise kontroll-loend on alustamine.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Azure‘i rakenduste registreerimisportaalis näete, millised rakendused kasutavad AAD Graphi. Soovitame teil kõigi rakenduste lähtekood läbi vaadata ja kui vaja, võtta ühendust ISV-de või rakendusepakkujatega. Microsofti tugiteenused võivad teile pakkuda ka teie rentniku kõigi AAD Graphide kasutuse loendit.
3. Rakenduses Microsoft Graph andmetele juurdepääsemiseks peab kasutaja või administraator andma sellele loa andmiseks õiged õigused. [Microsoft Graph permissions References](https://docs.microsoft.com/graph/permissions-reference) loetletakse kõigi Microsoft Graphi API-de põhikomplektiga seotud load. See sisaldab ka juhiseid selle kohta, kuidas kasutada lube.
