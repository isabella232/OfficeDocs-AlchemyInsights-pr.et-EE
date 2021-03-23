---
title: Autentimine teekidega töötamine
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
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035286"
---
# <a name="working-with-authentication-libraries"></a>Autentimine teekidega töötamine

Microsofti autentimise teegi (MSAL) probleemi lahendamiseks tehke järgmist soovitatud toiminguid.

1. **Töötamine MSAL**: [Microsofti identiteedi platvormi autentimine teegid](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) – selles artiklis kirjeldatakse mitme rakenduse tüüpi Microsofti autentimise teegi tuge. See sisaldab linke teegi lähtekoodi; kust saada oma rakenduse projekti pakett; ja kas teek toetab kasutaja sisselogimist (autentimine), juurdepääsu kaitstud Web API-de (autoriseerimine) või mõlemat.

2. **Autentimise tõrkeotsing**: MSAL toetab mitmeid autentimise voogusid eri rakenduse stsenaariumite jaoks. Olenevalt sellest, kuidas teie klientrakendus on loodud, saab MSAL kasutada ühte või mitut Microsofti identiteedi platvormi toetatud autentimise voogusid. Need vood võivad toota mitut tüüpi lube ja autoriseerimise koode ning nõuda nende töö tegemiseks erinevaid märke.

3. **Accessi märgid**: [Microsoft Identity Platform Accessi märked](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – saate teada, kuidas teie API saab kinnitada ja kasutada Accessi loaga olevaid nõudeid. Kõik selle artikli dokumendid, välja arvatud juhul, kui need on märgitud, rakenduvad ainult registreeritud API-de jaoks väljaantud märkide korral. Seda ei kohaldata Microsofti omanduses olevate API-de jaoks välja antud märkide suhtes, samuti ei saa neid märke kasutada selleks, et valideerida, kuidas Microsoft Identity Platform teie loodud API jaoks lube väljastab.

**Azure Active Directory autentimise teegi (ADAL) toe lõpp**

- **Alates 30 juunist 2020** ei lisa me enam ADAL ja Azure AD Graphi uusi funktsioone. Pakume endiselt tehnilist tuge ja turbevärskendusi, ent mitte enam funktsioonivärskendusi.
- **Alates 30 juuni 2022,** lõpetame ADAL ja Azure AD Graphi toe ning ei paku enam tehnilist tuge ega turvavärskendusi.
- Rakendused, mis kasutavad ADAL olemasolevatel OPERATSIOONISÜSTEEMI versioonidel, jätkavad tööd ka pärast seda, kuid ei *saa tehnilist tuge ega turvavärskendusi*.
- Azure AD Graphi rakendused ei pruugi pärast selle aja möödumist enam saada vastuseid Azure AD Graphi lõpp-punktist.

**ADAL migreerimine**

- Soovitame värskendada MSAL, millel on uusimad funktsioonid ja turvavärskendused.
- Kui kasutate Microsoft apps ' i, saate teada, et Microsoft on oma rakenduste migreerimise protsessis MSAL lõpptähtajaks, tagades, et nad saavad kasu MSAL pidevast turbest ja funktsioonide täiustustest.

1. [Lugege ADAL KKK-sid](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
2. [Siit saate teada, kuidas rakendusi ühe platvormi põhjal migreerida](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).
3. Kui teil on pärast rakenduse platvormile lisatud juhendi lugemist lisaküsimusi, saate postitada [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) sildiga [Azure-AD-ADAL-aegunud] või avada probleemi teegi github hoidlas. Iga teegi Repo lingid leiate teemast **MSAL ülevaade** artiklist [keeled ja raamistikud](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) .
4. **Kui vajate abi selle kohta, millised rakendused kasutavad ADAL**, soovitame teil kõik oma rakenduste lähtekoodi üle vaadata. Vajadusel REACH-iga sõltumatute tarkvara tarnijate (tarkvaratoode) või rakenduste pakkujatega. Samuti saab Microsofti tugi anda teile nimekirja kõigist neist mitte-Microsofti rakendustest teie rentnikkeskkonnas, mis kasutavad ADAL-i.







