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
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="b0e96-102">Microsoft Graphi API päring</span><span class="sxs-lookup"><span data-stu-id="b0e96-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="b0e96-103">See teema võib kehtida ka siis, kui arendajad kasutavad endiselt Azure AD Graph API-d.</span><span class="sxs-lookup"><span data-stu-id="b0e96-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="b0e96-104">Siiski on **tungivalt** soovitatav kasutada Microsoft Graphi kõigi kataloogide, identiteedi ja Accessi halduse stsenaariumite jaoks.</span><span class="sxs-lookup"><span data-stu-id="b0e96-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="b0e96-105">**Autentimise või autoriseerimisega seotud probleemid**</span><span class="sxs-lookup"><span data-stu-id="b0e96-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="b0e96-106">Kui teie rakendus ei saa Microsofti graafikule helistamiseks **märke hankida** , valige **probleem** , kui soovite selle teema kohta täpsemat abi ja tuge hankida Microsoft Graphi kategooria kaudu.</span><span class="sxs-lookup"><span data-stu-id="b0e96-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="b0e96-107">Kui rakenduses Microsoft Graph helistamisel kuvatakse rakenduse **401 või 403 lubamise tõrked** , **Valige selle teema** kohta täpsema abi ja toe hankimiseks Microsoft Graph API kategooria.</span><span class="sxs-lookup"><span data-stu-id="b0e96-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="b0e96-108">**Soovin kasutada rakendust Microsoft Graph, kuid pole kindel, kust alustada**</span><span class="sxs-lookup"><span data-stu-id="b0e96-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="b0e96-109">Lisateavet Microsoft Graphi kohta leiate järgmistest teemadest.</span><span class="sxs-lookup"><span data-stu-id="b0e96-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="b0e96-110">Microsoft Graphi ülevaade</span><span class="sxs-lookup"><span data-stu-id="b0e96-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="b0e96-111">Microsoft Graphi identiteedi ja Accessi halduse ülevaade</span><span class="sxs-lookup"><span data-stu-id="b0e96-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="b0e96-112">Microsoft Graphi rakenduste loomise alustamine</span><span class="sxs-lookup"><span data-stu-id="b0e96-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="b0e96-113">**Microsoft Graph Explorer** – Microsoft Graphi API-de testimine rentniku või demo rentniku jaoks</span><span class="sxs-lookup"><span data-stu-id="b0e96-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="b0e96-114">**Soovin kasutada rakendust Microsoft Graph, kuid see toetab ka v 1.0 kataloogi API-sid, mida vajan?**</span><span class="sxs-lookup"><span data-stu-id="b0e96-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="b0e96-115">Microsoft Graph on soovitatav API kataloogis, identiteedis ja Accessi halduses.</span><span class="sxs-lookup"><span data-stu-id="b0e96-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="b0e96-116">Siiski on võimalik, et Azure AD Graphis ja Microsoft Graphis on veel mõned lüngad.</span><span class="sxs-lookup"><span data-stu-id="b0e96-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="b0e96-117">Vaadake üle järgmised artiklid, kus on esile tõstetud kõige ajakohased erinevused teie valitud abistamiseks.</span><span class="sxs-lookup"><span data-stu-id="b0e96-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="b0e96-118">Ressursi tüübi erinevused Azure AD Graphis ja Microsoft Graphis</span><span class="sxs-lookup"><span data-stu-id="b0e96-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="b0e96-119">Azure AD Graphi ja Microsoft Graphi atribuutide erinevused</span><span class="sxs-lookup"><span data-stu-id="b0e96-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="b0e96-120">Azure AD ja Microsoft Graphi erinevuste meetod</span><span class="sxs-lookup"><span data-stu-id="b0e96-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="b0e96-121">***Kasutaja* objekti päringu korral on mitmed selle atribuudid puudu**</span><span class="sxs-lookup"><span data-stu-id="b0e96-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="b0e96-122">`GET https://graph.microsoft.com/v1.0/users` tagastab ainult 11 atribuuti, kuna Microsoft Graph automaatselt valib vaikimisi *kasutajate* atribuutide kogumi.</span><span class="sxs-lookup"><span data-stu-id="b0e96-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="b0e96-123">Kui vajate muid *kasutajate* atribuute, kasutage rakenduse vajaduste valimiseks $Select.</span><span class="sxs-lookup"><span data-stu-id="b0e96-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="b0e96-124">Proovige **Microsoft Graph Exploreris** esmalt.</span><span class="sxs-lookup"><span data-stu-id="b0e96-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="b0e96-125">**Mõned kasutaja atribuudi väärtused on *tühjad* , kuigi ma tean, et need on seatud**</span><span class="sxs-lookup"><span data-stu-id="b0e96-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="b0e96-126">Kõige tõenäolisem selgitus on see, et rakendusele anti *kasutaja. ReadBasic. kõik* õigused.</span><span class="sxs-lookup"><span data-stu-id="b0e96-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="b0e96-127">See võimaldab rakendusel lugeda piiratud kasutajate atribuute, mis tagastavad kõik muud atribuudid nulliga, isegi kui need on eelnevalt määratud.</span><span class="sxs-lookup"><span data-stu-id="b0e96-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="b0e96-128">Proovige anda rakenduse *kasutaja. Lugege* selle asemel kõiki õigusi.</span><span class="sxs-lookup"><span data-stu-id="b0e96-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="b0e96-129">Lisateavet leiate teemast [Microsoft Graph User permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span><span class="sxs-lookup"><span data-stu-id="b0e96-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="b0e96-130">**Mul on probleeme OData päringu parameetrite abil andmete filtreerimiseks minu päringutes**</span><span class="sxs-lookup"><span data-stu-id="b0e96-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="b0e96-131">Kui Microsoft Graph toetab paljusid OData päringu parameetreid, ei toeta paljud neist parameetritest täielikult kataloogiteenuse (ressursid, mis pärivad *directoryObject*) Microsoft Graphis.</span><span class="sxs-lookup"><span data-stu-id="b0e96-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="b0e96-132">Rakenduses Azure AD Graph olevad samad piirangud püsivad enamasti Microsoft Graphi rakenduses.</span><span class="sxs-lookup"><span data-stu-id="b0e96-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="b0e96-133">**Pole toetatud**: $count, $search ja $filter väärtus *null* või *Not Null*</span><span class="sxs-lookup"><span data-stu-id="b0e96-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="b0e96-134">**Pole toetatud**: $filter teatud atribuutidele (vt ressursside teemasid, mille atribuudid on filtreeritud)</span><span class="sxs-lookup"><span data-stu-id="b0e96-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="b0e96-135">**Pole toetatud**: saalefaili, filtreerimine ja sortimine samal ajal</span><span class="sxs-lookup"><span data-stu-id="b0e96-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="b0e96-136">**Pole toetatud**: seose filtreerimine.</span><span class="sxs-lookup"><span data-stu-id="b0e96-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="b0e96-137">Näiteks – leiad kõik Suurbritannias olevad inseneritööd.</span><span class="sxs-lookup"><span data-stu-id="b0e96-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="b0e96-138">**Osaline tugi**: $OrderBy *kasutaja* (ainult DisplayName ja userPrincipalName) ning *rühm*</span><span class="sxs-lookup"><span data-stu-id="b0e96-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="b0e96-139">**Osaline tugi**: $filter (toetab ainult *EQ*-, *startsWith* *-* *või* *ja piiratud)* tuge, $expand (ühe objekti seoste laiendamine annab kõik seosed, kuid objektide kogumi laiendamine on piiratud)</span><span class="sxs-lookup"><span data-stu-id="b0e96-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="b0e96-140">Lisateavet leiate teemast [vastuste kohandamine päringu parameetritega](https://docs.microsoft.com/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b0e96-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="b0e96-141">**Sissehelistamise API ei tööta – kus saab teha veel teste?**</span><span class="sxs-lookup"><span data-stu-id="b0e96-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="b0e96-142">**Microsoft Graph Explorer** – testige Microsoft Graphi API-sid rentniku või demo rentniku jaoks ja vaadake ka Microsoft Graphi Exploreri **päringute päringuid** .</span><span class="sxs-lookup"><span data-stu-id="b0e96-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="b0e96-143">**Andmete päringute korral tundub, et ma saan mittetäieliku andmete kogumi tagasi**</span><span class="sxs-lookup"><span data-stu-id="b0e96-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="b0e96-144">Kui päringute kogumik (nt *Kasutajad*), kasutab Microsoft Graph serveripoolse lehe limiite, et tulemid oleksid alati vaikimisi lehe suurusega.</span><span class="sxs-lookup"><span data-stu-id="b0e96-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="b0e96-145">Teie rakendus peaks alati eeldama, et teenusest tagastatud kollektsioonid on lehel.</span><span class="sxs-lookup"><span data-stu-id="b0e96-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="b0e96-146">Lisateavet leiate järgmistest teemadest.</span><span class="sxs-lookup"><span data-stu-id="b0e96-146">For more information, see:</span></span>

- [<span data-ttu-id="b0e96-147">Microsoft Graphi head tavad</span><span class="sxs-lookup"><span data-stu-id="b0e96-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="b0e96-148">Microsoft Graphi andmete kutsungi rakenduses</span><span class="sxs-lookup"><span data-stu-id="b0e96-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="b0e96-149">**Minu rakendus on liiga aeglane ja seda saab ka ahendada. Milliseid täiustusi saab teha?**</span><span class="sxs-lookup"><span data-stu-id="b0e96-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="b0e96-150">Olenevalt teie stsenaariumist on teie käsutuses mitmeid erinevaid võimalusi, mis aitavad teil oma rakendust rohkem teha, ja mõnel juhul on teenusel vähem altid (kui teete liiga palju kõnesid).</span><span class="sxs-lookup"><span data-stu-id="b0e96-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="b0e96-151">Lisateavet leiate järgmistest teemadest.</span><span class="sxs-lookup"><span data-stu-id="b0e96-151">To learn more, see:</span></span>

- [<span data-ttu-id="b0e96-152">Microsoft Graphi head tavad</span><span class="sxs-lookup"><span data-stu-id="b0e96-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="b0e96-153">Partiide taotlemine</span><span class="sxs-lookup"><span data-stu-id="b0e96-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="b0e96-154">Muutuste jälitus Delta päringu kaudu</span><span class="sxs-lookup"><span data-stu-id="b0e96-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="b0e96-155">Muudatustest teavitamine webhooks kaudu</span><span class="sxs-lookup"><span data-stu-id="b0e96-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="b0e96-156">Ahendamise juhised</span><span class="sxs-lookup"><span data-stu-id="b0e96-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="b0e96-157">**Kust leida lisateavet tõrgete ja teadaolevate probleemide kohta?**</span><span class="sxs-lookup"><span data-stu-id="b0e96-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="b0e96-158">Microsoft Graphi tõrgetele reageerimise teave</span><span class="sxs-lookup"><span data-stu-id="b0e96-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="b0e96-159">Microsoft Graphi teadaolevad probleemid</span><span class="sxs-lookup"><span data-stu-id="b0e96-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="b0e96-160">**Kus saab vaadata teenuse kättesaadavuse ja ühenduvuse olekut?**</span><span class="sxs-lookup"><span data-stu-id="b0e96-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="b0e96-161">Teenuste kättesaadavus ja Ühenduvus, millele pääseb juurde Microsoft Graphi kaudu, võib mõjutada Microsoft Graphi üldist kättesaadavust ja jõudlust.</span><span class="sxs-lookup"><span data-stu-id="b0e96-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="b0e96-162">Azure Active Directory teenuse tervist kontrollitakse [Azure ' i oleku lehel](https://azure.microsoft.com/status/)loetletud **turbe + identiteedi** teenuste olekut.</span><span class="sxs-lookup"><span data-stu-id="b0e96-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="b0e96-163">Office ' i teenuste jaoks, mis aitavad kaasa Microsoft Graphi, kontrollige [Office ' i teenuse tervise armatuurlaual](https://portal.office.com/adminportal/home#/servicehealth)loetletud teenuste olekut.</span><span class="sxs-lookup"><span data-stu-id="b0e96-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
