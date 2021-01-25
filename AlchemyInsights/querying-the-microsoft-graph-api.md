---
title: Microsoft Graphi API päring
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
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974285"
---
# <a name="querying-the-microsoft-graph-api"></a>Microsoft Graphi API päring

See teema võib kehtida ka siis, kui arendajad kasutavad endiselt Azure AD Graph API-d. Siiski on **tungivalt** soovitatav kasutada Microsoft Graphi kõigi kataloogide, identiteedi ja Accessi halduse stsenaariumite jaoks.

**Autentimise või autoriseerimisega seotud probleemid**

- Kui teie rakendus ei saa Microsofti graafikule helistamiseks **märke hankida** , valige **probleem** , kui soovite selle teema kohta täpsemat abi ja tuge hankida Microsoft Graphi kategooria kaudu.
- Kui rakenduses Microsoft Graph helistamisel kuvatakse rakenduse **401 või 403 lubamise tõrked** , **Valige selle teema** kohta täpsema abi ja toe hankimiseks Microsoft Graph API kategooria.

**Soovin kasutada rakendust Microsoft Graph, kuid pole kindel, kust alustada**

Lisateavet Microsoft Graphi kohta leiate järgmistest teemadest.

- [Microsoft Graphi ülevaade](https://docs.microsoft.com/graph/overview)
- [Microsoft Graphi identiteedi ja Accessi halduse ülevaade](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Microsoft Graphi rakenduste loomise alustamine](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – Microsoft Graphi API-de testimine rentniku või demo rentniku jaoks

**Soovin kasutada rakendust Microsoft Graph, kuid see toetab ka v 1.0 kataloogi API-sid, mida vajan?**

Microsoft Graph on soovitatav API kataloogis, identiteedis ja Accessi halduses. Siiski on võimalik, et Azure AD Graphis ja Microsoft Graphis on veel mõned lüngad. Vaadake üle järgmised artiklid, kus on esile tõstetud kõige ajakohased erinevused teie valitud abistamiseks.

- [Ressursi tüübi erinevused Azure AD Graphis ja Microsoft Graphis](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Azure AD Graphi ja Microsoft Graphi atribuutide erinevused](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Azure AD ja Microsoft Graphi erinevuste meetod](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

***Kasutaja* objekti päringu korral on mitmed selle atribuudid puudu**

`GET https://graph.microsoft.com/v1.0/users` tagastab ainult 11 atribuuti, kuna Microsoft Graph automaatselt valib vaikimisi *kasutajate* atribuutide kogumi. Kui vajate muid *kasutajate* atribuute, kasutage rakenduse vajaduste valimiseks $Select. Proovige **Microsoft Graph Exploreris** esmalt.

**Mõned kasutaja atribuudi väärtused on *tühjad* , kuigi ma tean, et need on seatud**

Kõige tõenäolisem selgitus on see, et rakendusele anti *kasutaja. ReadBasic. kõik* õigused. See võimaldab rakendusel lugeda piiratud kasutajate atribuute, mis tagastavad kõik muud atribuudid nulliga, isegi kui need on eelnevalt määratud. Proovige anda rakenduse *kasutaja. Lugege* selle asemel kõiki õigusi.

Lisateavet leiate teemast [Microsoft Graph User permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Mul on probleeme OData päringu parameetrite abil andmete filtreerimiseks minu päringutes**

Kui Microsoft Graph toetab paljusid OData päringu parameetreid, ei toeta paljud neist parameetritest täielikult kataloogiteenuse (ressursid, mis pärivad *directoryObject*) Microsoft Graphis. Rakenduses Azure AD Graph olevad samad piirangud püsivad enamasti Microsoft Graphi rakenduses.

1. **Pole toetatud**: $count, $search ja $filter väärtus *null* või *Not Null*
2. **Pole toetatud**: $filter teatud atribuutidele (vt ressursside teemasid, mille atribuudid on filtreeritud)
3. **Pole toetatud**: saalefaili, filtreerimine ja sortimine samal ajal
4. **Pole toetatud**: seose filtreerimine. Näiteks – leiad kõik Suurbritannias olevad inseneritööd.
5. **Osaline tugi**: $OrderBy *kasutaja* (ainult DisplayName ja userPrincipalName) ning *rühm*
6. **Osaline tugi**: $filter (toetab ainult *EQ*-, *startsWith* *-* *või* *ja piiratud)* tuge, $expand (ühe objekti seoste laiendamine annab kõik seosed, kuid objektide kogumi laiendamine on piiratud)

Lisateavet leiate teemast [vastuste kohandamine päringu parameetritega](https://docs.microsoft.com/graph/query-parameters).

**Sissehelistamise API ei tööta – kus saab teha veel teste?**

**Microsoft Graph Explorer** – testige Microsoft Graphi API-sid rentniku või demo rentniku jaoks ja vaadake ka Microsoft Graphi Exploreri **päringute päringuid** .

**Andmete päringute korral tundub, et ma saan mittetäieliku andmete kogumi tagasi**

Kui päringute kogumik (nt *Kasutajad*), kasutab Microsoft Graph serveripoolse lehe limiite, et tulemid oleksid alati vaikimisi lehe suurusega. Teie rakendus peaks alati eeldama, et teenusest tagastatud kollektsioonid on lehel.

Lisateavet leiate järgmistest teemadest.

- [Microsoft Graphi head tavad](https://docs.microsoft.com/graph/best-practices-concept)
- [Microsoft Graphi andmete kutsungi rakenduses](https://docs.microsoft.com/graph/paging)

**Minu rakendus on liiga aeglane ja seda saab ka ahendada. Milliseid täiustusi saab teha?**

Olenevalt teie stsenaariumist on teie käsutuses mitmeid erinevaid võimalusi, mis aitavad teil oma rakendust rohkem teha, ja mõnel juhul on teenusel vähem altid (kui teete liiga palju kõnesid).

Lisateavet leiate järgmistest teemadest.

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
