---
title: Microsoft Graph API päringud
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
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923235"
---
# <a name="querying-the-microsoft-graph-api"></a>Microsoft Graph API päringud

See teema võib kehtida ka arendajatele, kes kasutavad endiselt Azure AD Graph API-d. Siiski on tungivalt **soovitatav** kasutada Microsoft Graph kõiki oma kataloogi-, identiteedi- ja juurdepääsuhalduse stsenaariume.

**Autentimis- või autoriseerimisprobleemid**

- Kui teie rakendus ei **saa** microsoft Graph'ile helistamiseks tõendeid hankida, valige selle teema kohta konkreetsema spikri ja toe saamiseks probleem microsoft Graph-kategooria juurdepääsulubade **(autentimine)** kasutamisel.
- Kui teie rakendus saab Microsoft Graph'ile helistamisel **401 või 403** autoriseerimistõrkeid, valige selle teema kohta lisateabe saamiseks kategooria Juurdepääsu keelamine **(autoriseerimine)** Microsoft Graph API.

**Soovin kasutada Microsoft Graph, kuid pole kindel, kust alustada**

Lisateavet Microsoft Graph kohta leiate teemast

- [Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Microsoft Graph rakenduste loomise alustamine](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – Microsoft Graph API-de testimine rentniku rentnikus või demo rentnikus

**Soovin kasutada Microsoft Graph, kuid kas see toetab v1.0 kataloogi API-sid, mida vajan?**

Microsoft Graph on soovitatav API kataloogi-, identiteedi- ja juurdepääsuhalduse jaoks. Siiski on Azure AD-d ja Microsoft Graph vahel veel Graph. Vaadake üle järgmised artiklid, mis tõstavad esile kõige aja ajasemad erinevused, mis aitavad teil valida.

- [Ressursitüübi erinevused Azure AD Graph Ja Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Azure AD Graph Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Azure AD ja Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Kui kasutajaobjekti kohta *päringuid teen,* on paljud selle atribuudid puudu**

`GET https://graph.microsoft.com/v1.0/users`Tagastab ainult 11 atribuuti, Graph Microsoft valib automaatselt  tagasipöördumiseks kasutaja atribuutide vaikekomplekti. Kui teil on vaja *muid kasutajaasuvaid* atribuute, $select valige atribuudid, mida teie rakendus vajab. Proovige seda esmalt **Microsoft Graph Exploreris.**

**Mõned kasutaja atribuudiväärtused on *nullväärtused,* kuigi ma tean, et need on määratud**

Kõige tõenäolisem selgitus on see, et rakendusele oli antud *User.ReadBasic.All* õigus. See võimaldab rakendusel lugeda piiratud kasutajaa atribuute, tagastades kõik muud atribuudid tühiväärtusena isegi siis, kui need on varem määratud. Proovige anda selle asemel *rakendusele User.Read.All* õigus.

Lisateavet leiate teemast [Microsoft Graph kasutajaõigused.](https://docs.microsoft.com/graph/permissions-reference#user-permissions)

**Mul on probleeme OData päringuparameetrite kasutamisega päringuandmete filtreerimiseks minu päringutes**

Kuigi Microsoft Graph toetab paljusid OData päringuparameetreid, ei toeta Microsoft Graph kataloogiteenused (kataloogist *Pärivad* ressursid) paljusid neid parameetreid täielikult. Azure AD-s kehtivad samad Graph Microsoft Graph.

1. **Pole toetatud:**$count, $search ja $filter *on* tühiväärtused või *mitte tühiväärtused*
2. **Pole toetatud:**$filter atribuudid (vt ressursiteemasid, mille atribuudid on filtreeritavad)
3. **Pole toetatud:** korraga saalimine, filtreerimine ja sortimine
4. **Pole toetatud:** seose filtreerimine. Näiteks : otsige üles kõik Ühendkuningriigis asuvad insenerirühma liikmed.
5. **Osaline tugi:**$orderby *(ainult* displayName ja userPrincipalName) ja *rühm*
6. **Osaline tugi:**$filter (toetab ainult *eq* *,* algab koos *või* *,* ja ja ja piiras *mis* tahes ) tuge, $expand (ühe objekti seoste laiendamine tagastab kõik seosed, kuid objektide seoste kogumi laiendamine on piiratud)

Lisateavet leiate teemast Vastuste [kohandamine päringuparameetrite abil.](https://docs.microsoft.com/graph/query-parameters)

**Api, kuhu ma helistan, ei tööta – kus saab teha rohkem testimist?**

**Microsoft Graph Explorer** – microsoft Graph API-sid oma rentnikus või demo  rentnikus ning tutvuge microsoft Graph Exploreri näidispäringutega.

**Andmepäringu korral tundub, et saan tagasi mittetäieliku andmekomplekti**

Kui küsite kogumilt (nt *kasutajatelt),* kasutab Microsoft Graph serveripoolseid lehepiiranguid, nii et tulemid tagastatakse alati lehe vaikesuurusega. Teie rakendus peaks alati eeldama teenusest tagastatud kogumite lehte.

Lisateavet leiate järgmistest teemadest.

- [Microsoft Graph head tavad](https://docs.microsoft.com/graph/best-practices-concept)
- [Microsoft Graph andmete saalimine rakenduses](https://docs.microsoft.com/graph/paging)

**Minu rakendus on liiga aeglane ja aheneb ka. Milliseid täiustusi saan teha?**

Olenevalt teie stsenaariumist on teie käsutuses mitmesugused võimalused, et muuta teie rakendus rohkem esinejaks ja mõnel juhul on teenuse ahendamise võimalus väiksem (kui teete liiga palju kõnesid).

Lisateavet leiate järgmistest teemadest.

- [Microsoft Graph head tavad](https://docs.microsoft.com/graph/best-practices-concept)
- [Pakketaotlused](https://docs.microsoft.com/graph/json-batching)
- [Muutuste jälitamine deltapäringu kaudu](https://docs.microsoft.com/graph/delta-query-overview)
- [Muudatustest teavitatakse veebihoobide kaudu](https://docs.microsoft.com/graph/webhooks)
- [Ahendamise juhised](https://docs.microsoft.com/graph/throttling)

**Kust leida lisateavet tõrgete ja teadaolevate probleemide kohta?**

- [Microsoft Graph tõrkevastuse teave](https://docs.microsoft.com/graph/errors)
- [Teadaolevad microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Kus saab kontrollida teenuse kättesaadavuse ja ühenduvuse olekut?**

Microsoft Graph kaudu juurdepääsetud teenuste kättesaadavus ja ühenduvus võivad mõjutada Microsofti teenuste üldist kättesaadavust ja Graph.

- Teenuse Azure Active Directory seisundi tagamiseks kontrollige Azure'i olekulehel loetletud turbe- ja [identiteediteenuste olekut.](https://azure.microsoft.com/status/) 
- Kui Office microsoft Graph, kontrollige teenuse seisundi [armatuurlaual Office teenuste olekut.](https://portal.office.com/adminportal/home#/servicehealth)
