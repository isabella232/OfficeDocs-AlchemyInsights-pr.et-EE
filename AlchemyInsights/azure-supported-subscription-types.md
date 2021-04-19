---
title: Toetatud tellimusetüübid
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6675"
ms.openlocfilehash: dcf5855bff8725ea746196c1f07d689ce1797f8c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820678"
---
# <a name="supported-subscription-types"></a>Toetatud tellimusetüübid

Edasiseks jätkamiseks vaadake üle toetatud tellimusetüübid.

[Toetatud tellimusetüübid](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Arvelduse omandiõiguse ülekandmine**

Azure'i [portaal selle](https://ms.portal.azure.com/) arvelduskonto konto administraatorina, mille tellimust soovite üle kanda

- Otsige üksusest **Kuluhaldus ja arveldus**. Valige **vasakpoolsel paanil** Tellimused. Olenevalt juurdepääsust on võimalik, et peate valima arveldusulatuse ja seejärel valiku **Tellimused** või **Azure’i tellimused**.
- Valige üleantud tellimuse arvelduse omandiõiguse üleandmine
- Sisestage selle kasutaja meiliaadress, kes on selle konto arveldusadministraator, kes saab tellimuse uueks omanikuks, ja seejärel valige **saada üleviimistaotlus**
- Kasutajale saadetakse meil koos juhtnööridega teie ülekandmistaotluse läbivaatamiseks. Ülekandmistaotluse kinnitamiseks peab kasutaja valima meilis toodud lingi ja järgima juhtnööre.

Märkus. Kui kannate tellimuse arvelduse omandiõiguse üle kasutaja kontole teises Azure AD rentnikus, eemaldatakse jäädavalt kõik rollipõhised juurdepääsu juhtimise [(RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) ülesanded tellimuse ressursside haldamiseks. Ainult uuel omanikul on juurdepääs tellimuse ressursside haldamiseks. Lisateavet leiate teemast [Tellimuse üleviimine kasutajale teises Azure AD rentnikus.](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)

**Tellimuse omandiõiguse üleandmine**

Tellimuse omandiõiguse ülemineku eeltingimused on rollipõhine juurdepääs (RBAC), et hallata tellimuse ressursse, kaotavad juurdepääsu. Lisateavet rentnikule olemasoleva tellimuse lisamise kohta leiate teemast Azure'i tellimuse [seostamine azure Active Directoryga](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support)või selle lisamine.

- Praeguse arveldustsükli olemasoleva tasumata summaga tellimuse üleviimist uuele maksevahendile uuele kontole üle ei kanta. Ainus teave, mis on uuel kontol kasutajatele kättesaadav, on teie tellimuse viimase kuu hind. Ülejäänud kasutus- ja arveldusajalugu ei edastata tellimusega.
- Enterprise Agreementi (EA) tellimuste arvelduse omandiõiguse üleandmine on praegu toetatud ainult ettevõttelepingu portaalis.
- Krediidile suunatud tellimuse (nagu Visual Studio, BizSpark, Microsoft Partner Network) üleviimine uuele kasutajale nõuab üleviimistaotluse aktsepteerimiseks Visual Studio/Microsofti partnerivõrgu litsentsi.
- Kõik ressursid (nt virtuaalarvutid, kettad ja veebisaidid) teisaldatakse uuele kontole edukalt. Rentnikuülese tellimuse üleviimine võib mõjutada järgmisi ressursse.

**Azure AD domeeniteenused**

Azure'i võtmehoidlad

- [SQL-iga seotud kasutajaid ja](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) andmebaase võib mõjutada, eriti kui klient kasutab Azure Active Directoryga seotud autentimist
- **Rakenduseteenused,** mis on konfigureeritud Azure Active Directory autentimisega, võivad mõjutada
- **Visual Studio meeskond** Azure'i tellimustega ühendatud teenusekontod võivad ühendatud Azure'i tellimuse tühistamisel ajutiselt juurdepääsu kaotada.

**Soovitatud dokumendid**

Pärast arvelduse omanikuks tunnistamist tehke järgmist.

- Arvelduse omandiõiguse säilitamiseks, kuid tellimuse tüübi muutmiseks lugege järgmist. [Azure'i tellimuse vahetamine teise pakkumisega](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Visual Studio, Microsoft Partner Networki ja Pay as you go arendus-/testtellimuste ülekandmine](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Enterprise Agreementi (EA) tellimuste arvelduse omandiõiguse üleandmine](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Omanduse ülekandmise KKK](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Omanduse ülekandmise probleemide tõrkeotsing](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)