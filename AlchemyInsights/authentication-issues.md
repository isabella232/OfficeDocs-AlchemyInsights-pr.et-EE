---
title: Autentimise probleemid
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: 53bd0d8f8edaead519d0282239d3a6d338b297b9
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974310"
---
# <a name="authentication-issues"></a>Autentimise probleemid

**Kas otsite teavet Azure Active Directory (Azure AD) turbelubade teenusest (STS) tagastatud AADSTS tõrkekoodidest?** Lugege artiklit [AZURE ad autentimine ja autoriseerimise tõrkekoodid](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) , et leida AADSTS, parandusi ja muid soovitatud lahendusi.

Autoriseerimise tõrked võivad olla tingitud mitmest erinevast probleemist, millest enamik tekitab 401 või 403 tõrke. Näiteks järgmised probleemid võivad anda loa tõrkeid:

- Ebaõiged juurdepääsuluba [omandavad vood](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- Halvasti konfigureeritud [õiguste ulatused](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- [Nõusoleku](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent) puudumine

Levinud autoriseerimise tõrgete lahendamiseks proovige allpool toodud juhiseid, mis vastavad kõige paremini teie saadud tõrkele. Teile kuvatakse tõrketeade, mida võidakse kasutada rohkem kui üks samm.

- **401 lubamatu tõrge: kas teie luba kehtib?**

Veenduge, et teie rakendus esitaks taotluse osana Microsoft Graphile kehtiva juurdepääsuluba. See tõrge tähendab sageli, et juurdepääsuluba võib olla puudu HTTP autentimine taotluse päises või et see on kehtetu või aegunud. Soovitame kasutada Accessi turbelubade omandamiseks Microsofti autentimise teeki (MSAL). See tõrge võib ilmneda juhul, kui proovite kasutada isiklikule Microsofti kontole antud volitatud juurdepääsuluba, et pääseda juurde API-ile, mis toetab ainult töö-või kooli kontosid (organisatsioonilised kontod).

**403 keelatud tõrge: Kas olete valinud õige õiguste kogumi?**

Veenduge, et olete taotlenud rakenduse Microsoft Graph API-l põhinevaid õigeid kasutajaõigusi. Soovitatavad kõige vähem privilegeeritud õigused on saadaval kõigis Microsoft Graphi API standardmeetodite teemades. Lisaks sellele peab kasutaja või administraator need õigused andma. Lubade andmine toimub tavaliselt loa lehe kaudu või Azure ' i portaali rakenduse registreerimis Blade kasutamise kaudu. Klõpsake rakenduse **sätete** Blade nuppu **nõutavad load** ja seejärel käsku **Anna õigustele**. Lisateavet leiate järgmistest teemadest.

- [Microsoft Graphi load](https://docs.microsoft.com/graph/permissions-reference) 
- [Azure AD kasutajaõiguste ja nõusoleku mõistmine](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**403 keelatud tõrge: kas teie rakendus omandas tõendi valitud õigustele vastamiseks?**

Veenduge, et taotletud või antud õiguse tüübid vastavad teie rakenduse omandatava juurdepääsuloa tüübile. Võib-olla taotlete ja lubate rakenduse kasutusõigusi, kuid kasutate delegeeritud interaktiivse koodi voo märkide asemel kliendi mandaatide voogude märke, või taotlete ja annate delegeeritud õiguseid, kuid kasutate delegeeritud koodi voo asemel kliendi mandaatide voogude märke.

Lisateavet märkide hankimisega seotud Lisateavet leiate järgmistest teemadest.

- [Juurdepääsu saamine kasutajate nimel ja delegeeritud õigustest](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v 2.0-OAuthi 2,0 loa koodi voog](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Juurdepääsu saamine kasutajata (Daemon Service) ja rakenduse kasutusõigused](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v 2.0-OAuthi 2,0 kliendi mandaatide voog](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403 keelatud tõrge: parooli ennistamine**

Praegu ei ole rakenduse luba Daemon Service-to-teenuse õigusi, mis lubavad kasutaja paroole uuesti määrata. Neid API-sid toetatakse ainult interaktiivse delegeeritud koodi abil, millel on sisse logitud administraator. Lisateavet leiate teemast [Microsoft Graphi load](https://docs.microsoft.com/graph/permissions-reference).

**403 keelatud: kas kasutajal on juurdepääs ja need on litsentsitud?**

Delegeeritud koodi voogude korral hindab Microsoft Graph, kas taotlus on lubatud, võttes aluseks rakenduse antud õigustele ja sisselogitud kasutaja õigustele. Üldiselt näitab see tõrge, et kasutajal pole piisavalt õigusi taotluse tegemiseks **või** kui kasutaja ei ole litsentsitud andmetele juurdepääsetav. Taotlust saab edukalt teha ainult selliste kasutajatega, kellel on nõutavad load või litsentsid.

**403 keelatud: kas valisite õige ressursi API?**

API-teenused (nt Microsoft Graph) kontrollivad *, et saadud* juurdepääsuluba (sihtrühm) vastab väärtusele, mida ta endale ootab, ja kui mitte, kuvatakse 403 keelatud tõrge. Sellest tõrkest tulenev levinud viga proovib kasutada Azure AD Graph API-de, Outlooki API-de või SharePointi/OneDrive ' i API-de jaoks saadud tõendit, et helistada Microsoft Graphile (või vastupidi). Veenduge, et teie rakenduse ressurss (või rakendusala) omandaks tõendi selle kohta, mis vastab rakenduse jaoks kasutatavale API-ile.

**400 halb taotlus või 403 keelatud: kas kasutaja täidab oma asutuse tingimusjuurdepääsu (CA) poliitika?**

Asutuse tingimusjuurdepääsu (CA) poliitika põhjal võidakse rakenduse Microsoft Graph ressurssidele juurdepääsuks teie rakenduse kaudu vaidlustada lisateavet, mida teie rakendus algselt soetatud juurdepääsuluba ei kasuta. Sellisel juhul saab teie rakendus 400, **millel on *interaction_required*** tõrge Accessi turbelubade omandamise ajal või **403, kus on** Microsoft Graphi helistamisel insufficient_claims tõrge. Mõlemal juhul sisaldab tõrketeade lisateavet, mida saab volitatud lõpp-punkti kaudu esitada, et vaidlustada kasutaja lisateavet (nt mitme teguri autentimine või seadme registreerimine).

Lisateavet tingimusliku juurdepääsu kohta leiate järgmistest teemadest.

- [MSAL abil tingimusjuurdepääsu probleemide käsitlemine](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Azure Active Directory rakenduse arendaja juhised tingimusjuurdepääsu jaoks](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Azure Active Directory autentimise teegi (ADAL) ja AZURE ad Graph API (AAD Graph) _ toe lõppemine_*

- Alates 30 juunist 2020 ei lisa me enam Azure Active Directory autentimise teeki (ADAL) ja Azure AD Graph API-d (AAD Graph) uusi funktsioone. Jätkame tehnilise toe ja turvavärskenduste esitamist, kuid ei paku enam funktsioonide värskendusi.
- Alates 30 juunist 2022, lõpetame ADAL ja AAD graafiku toe ning ei paku enam tehnilist tuge ega turvavärskendusi.
    - Rakendused, mis kasutavad ADAL olemasolevatel OPERATSIOONISÜSTEEMI versioonidel, jätkavad tööd ka pärast seda, kuid ei saa tehnilist tuge ega turvavärskendusi.
    - Pärast seda, kui see aeg on AAD Graphiga rakendusi saanud, ei pruugi see enam saada vastuseid AAD Graph Endpoint.

_ *ADAL migreerimine**

Soovitame värskendada [Microsoft Authenticationi teeki (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), millel on uusimad funktsioonid ja turvavärskendused. See soovitus on kontekstis, mille Microsoft migreerib oma rakendused MSAL lõpptähtajaks. Microsoft apps ' i migreerimise eesmärk MSAL on tagada, et rakendused saavad kasu MSAL pidevast turbest ja funktsioonide täiustustest.

- [Lugege ADAL KKK-sid](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Vaadake, kuidas rakendusi ühe platvormi põhjal migreerida](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Kui vajate abi selle kohta, millised rakendused kasutavad ADAL, soovitame teil kõigi rakenduste lähtekoodi üle vaadata ja vajaduse korral jõuda kõigi sõltumatute tarkvara tarnijate (tarkvaratoode) või rakenduste pakkujatega. Microsofti tugiteenused võivad anda teile ka kõigi teie rentniku jaoks mitte-Microsofti ADAL rakenduste loendi.

**AAD Graphi migreerimine**

Kui teil on rakenduses AAD Graph kasutatavaid rakendusi, järgige meie juhiseid [AZURE ad Graphi rakenduste migreerimiseks Microsoft Graphi](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Meie migreerimise kontroll-loend on](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)alustamine. 
- Teie Azure ' i rakenduse registreerimise portaal näitab, millised rakendused kasutavad AAD graafikut. Soovitame üle vaadata kõik rakenduste lähtekoodi ja vajaduse korral jõuda mõnele tarkvaratoode või rakenduste pakkujale. Microsofti tugiteenused võivad anda teile ka teavet kõigi AAD Graphide kasutuse kohta rentniku jaoks.

 










