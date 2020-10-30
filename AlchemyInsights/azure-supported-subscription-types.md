---
title: Toetatud tellimuse tüübid
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6675"
ms.openlocfilehash: 46bc60435c3f8477e9f274d90c39d0f1c6a523c6
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807567"
---
# <a name="supported-subscription-types"></a>Toetatud tellimuse tüübid

Jätkamiseks vaadake üle toetatud tellimuse tüübid.

[Toetatud tellimuse tüübid](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Arvelduse omandiõiguse üleviimine**

Azure ' i portaal [konto administraatorina](https://ms.portal.azure.com/) , mille tellimust soovite üle viia

- Otsige **kulude haldus + arveldus** . Valige vasakpoolsel paanil **tellimused** . Olenevalt Accessist peate võib-olla valima arveldamise ulatuse ja seejärel **tellimused** või **Azure ' i tellimused** .
- Valige üle kantava tellimuse ülekandmise arveldamise omanik
- Sisestage selle kasutaja meiliaadress, kes on tellimuse uueks omanikuks oleva konto arveldamise administraator ja seejärel valige **saada edastuse taotlus**
- Kasutaja saab teie edastuse taotluse läbivaatamiseks meili teel juhiseid. Edastuse taotluse kinnitamiseks valib kasutaja meilisõnumis oleva lingi ja järgib juhiseid.

Märkus: Kui edastate oma tellimuse arveldamise omandiõiguse mõnele teisele Azure AD rentniku kontole, eemaldatakse kõik [rolli-põhise juurdepääsu juhtimise (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) ülesanded tellimuse ressursside haldamiseks jäädavalt. Ainult uuel omanikul on juurdepääs tellimuse ressursside haldamiseks. Lisateavet leiate teemast [tellimuse edastamine kasutajale teise AZURE ad rentniku](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)jaoks.

**Tellimuse omandiõiguse üleviimine**

Tellimuse omandiõiguse ülekandmise eeldused (RBAC), mis haldavad tellimuse ressursse, kaotavad juurdepääsu. Lisateavet rentniku jaoks olemasoleva tellimuse lisamise kohta leiate teemast Azure ' i [tellimuse lisamine Azure ' i Active Directorys](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Tellimuse üleminekut olemasolevast arvelduse tsüklist praegusest arvelduse tsüklist ei edastata uuele maksevahendile uues kontos. Ainult uue konto kasutajatele saadaolev teave on teie tellimuse viimase kuu hind. Ülejäänud kasutuse ja arvelduste ajalugu ei edasta paketti.
- Enterprise Agreement (EA) tellimuste omandiõiguse ülekandmise hetkel toetatakse ainult ettevõtteportaali portaalis
- Krediidile orienteeritud tellimuse (nt Visual Studio, BizSpark, Microsoft Partner Network for uuele kasutajale) üleviimine eeldab, et Visual Studio/Microsoft Partner Network litsents aktsepteerib edastuse taotlust
- Kõik ressursid (nt virtuaalsed masinad, kettad ja veebisaidid) edastatakse uuele kontole edukalt. Rentniku tellimuse üleviimine võib mõjutada järgmisi ressursse.

**Azure AD Domain Services**

Azure ' i võtmete hoidlad

- [SQL-i seotud kasutajad ja andmebaasid](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) võivad mõjutada, eriti juhul, kui klient kasutab Azure Active Directory seotud autentimist
- Azure Active Directory autentimisega konfigureeritud **rakenduse teenused** võivad mõjutada
- **Visual Studio meeskond** Azure ' i abonemendiga ühendatud teenuste kontod võivad ajutiselt kaotada juurdepääsu, kui ühendatud Azure ' i tellimus on tühistatud

**Soovitatavad dokumendid**

Toimingud pärast arvelduse omanikuõiguse aktsepteerimist.

- Arvete omandiõiguse säilitamiseks, kuid oma tellimuse tüübi muutmiseks vaadake teemat: [Azure ' i tellimuse teise pakkumise aktiveerimine](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Üle Visual Studio, Microsoft Partner Network (MPN) ja maksta, kui lähete dev/test tellimused](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Enterprise Agreementi (EA) tellimuste arveldamise omandiõiguse üleviimine](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Omandiõiguse ülekandmise KKK](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Omandiõiguse ülekandmise probleemide tõrkeotsing](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)