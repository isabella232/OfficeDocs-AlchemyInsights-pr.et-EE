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
# <a name="microsoft-graph-api-issues"></a><span data-ttu-id="8beb4-102">Microsoft Graphi API probleemid</span><span class="sxs-lookup"><span data-stu-id="8beb4-102">Microsoft Graph API issues</span></span>

<span data-ttu-id="8beb4-103">See teema võib kehtida ka siis, kui arendajad kasutavad endiselt Azure AD Graph API-d.</span><span class="sxs-lookup"><span data-stu-id="8beb4-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="8beb4-104">Siiski on **tungivalt** soovitatav kasutada Microsoft Graphi kõigi kataloogide, identiteedi ja Accessi halduse stsenaariumite jaoks.</span><span class="sxs-lookup"><span data-stu-id="8beb4-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="8beb4-105">**Autentimise või autoriseerimisega seotud probleemid**</span><span class="sxs-lookup"><span data-stu-id="8beb4-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="8beb4-106">Kui teie rakendus ei saa Microsofti graafikule helistamiseks **märke hankida** , valige **probleem** , kui soovite selle teema kohta täpsemat abi ja tuge hankida Microsoft Graphi kategooria kaudu.</span><span class="sxs-lookup"><span data-stu-id="8beb4-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="8beb4-107">Kui rakenduses Microsoft Graph helistamisel kuvatakse rakenduse **401 või 403 lubamise tõrked** , **Valige selle teema** kohta täpsema abi ja toe hankimiseks Microsoft Graph API kategooria.</span><span class="sxs-lookup"><span data-stu-id="8beb4-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="8beb4-108">**Soovin kasutada rakendust Microsoft Graph, kuid pole kindel, kust alustada**</span><span class="sxs-lookup"><span data-stu-id="8beb4-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

- [<span data-ttu-id="8beb4-109">Microsoft Graphi ülevaade</span><span class="sxs-lookup"><span data-stu-id="8beb4-109">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="8beb4-110">Microsoft Graphi identiteedi ja Accessi halduse ülevaade</span><span class="sxs-lookup"><span data-stu-id="8beb4-110">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="8beb4-111">Microsoft Graphi rakenduste loomise alustamine</span><span class="sxs-lookup"><span data-stu-id="8beb4-111">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="8beb4-112">**Microsoft Graph Explorer** – Microsoft Graphi API-de testimine rentniku või demo rentniku jaoks</span><span class="sxs-lookup"><span data-stu-id="8beb4-112">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="8beb4-113">**Soovin kasutada rakendust Microsoft Graph, kuid see toetab ka v 1.0 kataloogi API-sid, mida vajan?**</span><span class="sxs-lookup"><span data-stu-id="8beb4-113">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="8beb4-114">Microsoft Graph on soovitatav API kataloogis, identiteedis ja Accessi halduses.</span><span class="sxs-lookup"><span data-stu-id="8beb4-114">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="8beb4-115">Siiski on võimalik, et Azure AD Graphis ja Microsoft Graphis on veel mõned lüngad.</span><span class="sxs-lookup"><span data-stu-id="8beb4-115">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="8beb4-116">Vaadake üle järgmised artiklid, kus on esile tõstetud kõige ajakohased erinevused teie valitud abistamiseks.</span><span class="sxs-lookup"><span data-stu-id="8beb4-116">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="8beb4-117">Ressursi tüübi erinevused Azure AD Graphis ja Microsoft Graphis</span><span class="sxs-lookup"><span data-stu-id="8beb4-117">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="8beb4-118">Azure AD Graphi ja Microsoft Graphi atribuutide erinevused</span><span class="sxs-lookup"><span data-stu-id="8beb4-118">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="8beb4-119">Azure AD ja Microsoft Graphi erinevuste meetod</span><span class="sxs-lookup"><span data-stu-id="8beb4-119">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="8beb4-120">**API, mida ma helistan, ei tööta – kus saab teha veel teste?**</span><span class="sxs-lookup"><span data-stu-id="8beb4-120">**The API I am calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="8beb4-121">**Microsoft Graph Explorer** – testige Microsoft Graphi API-sid rentniku või demo rentniku jaoks ja vaadake ka Microsoft Graphi Exploreri **päringute päringuid** .</span><span class="sxs-lookup"><span data-stu-id="8beb4-121">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="8beb4-122">**Minu rakendus on liiga aeglane ja seda saab ka ahendada. Milliseid täiustusi saab teha?**</span><span class="sxs-lookup"><span data-stu-id="8beb4-122">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="8beb4-123">Olenevalt teie stsenaariumist on teie käsutuses mitmeid võimalusi, mis aitavad teil oma rakendust rohkem teha, ja mõnel juhul on teenusel vähem altid (kui teete liiga palju kõnesid).</span><span class="sxs-lookup"><span data-stu-id="8beb4-123">Depending on your scenario, there are a variety of options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

- [<span data-ttu-id="8beb4-124">Microsoft Graphi head tavad</span><span class="sxs-lookup"><span data-stu-id="8beb4-124">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="8beb4-125">Partiide taotlemine</span><span class="sxs-lookup"><span data-stu-id="8beb4-125">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="8beb4-126">Muutuste jälitus Delta päringu kaudu</span><span class="sxs-lookup"><span data-stu-id="8beb4-126">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="8beb4-127">Muudatustest teavitamine webhooks kaudu</span><span class="sxs-lookup"><span data-stu-id="8beb4-127">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="8beb4-128">Ahendamise juhised</span><span class="sxs-lookup"><span data-stu-id="8beb4-128">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="8beb4-129">**Kust leida lisateavet tõrgete ja teadaolevate probleemide kohta?**</span><span class="sxs-lookup"><span data-stu-id="8beb4-129">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="8beb4-130">Microsoft Graphi tõrgetele reageerimise teave</span><span class="sxs-lookup"><span data-stu-id="8beb4-130">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="8beb4-131">Microsoft Graphi teadaolevad probleemid</span><span class="sxs-lookup"><span data-stu-id="8beb4-131">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="8beb4-132">**Kus saab vaadata teenuse kättesaadavuse ja ühenduvuse olekut?**</span><span class="sxs-lookup"><span data-stu-id="8beb4-132">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="8beb4-133">Teenuste kättesaadavus ja Ühenduvus, millele pääseb juurde Microsoft Graphi kaudu, võib mõjutada Microsoft Graphi üldist kättesaadavust ja jõudlust.</span><span class="sxs-lookup"><span data-stu-id="8beb4-133">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="8beb4-134">Azure Active Directory teenuse tervist kontrollitakse [Azure ' i oleku lehel](https://azure.microsoft.com/status/)loetletud **turbe + identiteedi** teenuste olekut.</span><span class="sxs-lookup"><span data-stu-id="8beb4-134">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="8beb4-135">Office ' i teenuste jaoks, mis aitavad kaasa Microsoft Graphi, kontrollige [Office ' i teenuse tervise armatuurlaual](https://portal.office.com/adminportal/home#/servicehealth)loetletud teenuste olekut.</span><span class="sxs-lookup"><span data-stu-id="8beb4-135">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="8beb4-136">Microsoft Graphi loa tõrked võivad olla tingitud mitmest erinevast probleemist, millest enamik tekitab 401 või 403 tõrke.</span><span class="sxs-lookup"><span data-stu-id="8beb4-136">Microsoft Graph authorization errors can be a result of several different issues, most of which generate a 401 or 403 error.</span></span> <span data-ttu-id="8beb4-137">Näiteks võib järgmine tõrketeade olla järgmine:</span><span class="sxs-lookup"><span data-stu-id="8beb4-137">For example, the following can all lead to authorization errors:</span></span>

- <span data-ttu-id="8beb4-138">valed [pääsutõendi hankimisvood](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span><span class="sxs-lookup"><span data-stu-id="8beb4-138">Incorrect [access token acquisition flows](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span></span>
- <span data-ttu-id="8beb4-139">kehvasti konfigureeritud [lubade ulatused](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span><span class="sxs-lookup"><span data-stu-id="8beb4-139">Poorly configured [permission scopes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span></span>
- <span data-ttu-id="8beb4-140">puuduv [nõusolek](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span><span class="sxs-lookup"><span data-stu-id="8beb4-140">Lack of [consent](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span></span>

<span data-ttu-id="8beb4-141">\**_Azure Active Directory autentimisteegi (ADAL) ja Azure AD Graphi API (AAD Graphi) tootetoe lõpp_* _</span><span class="sxs-lookup"><span data-stu-id="8beb4-141">\**_End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)_* _</span></span>

<span data-ttu-id="8beb4-142">_ \* Alates 30 juuni, 2020 \* \*, me ei lisa enam uusi funktsioone ADAL ja Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="8beb4-142">_\*Starting June 30th, 2020\*\*, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="8beb4-143">Pakume endiselt tehnilist tuge ja turbevärskendusi, ent mitte enam funktsioonivärskendusi.</span><span class="sxs-lookup"><span data-stu-id="8beb4-143">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="8beb4-144">**Alates 30 juuni 2022**, lõpetame ADAL ja Azure AD Graphi toe ning ei paku enam tehnilist tuge ega turvavärskendusi.</span><span class="sxs-lookup"><span data-stu-id="8beb4-144">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="8beb4-145">Rakendused, mis kasutavad ADAL olemasolevatel OPERATSIOONISÜSTEEMI versioonidel, jätkavad tööd ka pärast seda, kuid ei *saa tehnilist tuge ega turvavärskendusi*.</span><span class="sxs-lookup"><span data-stu-id="8beb4-145">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="8beb4-146">Azure AD Graphi rakendused ei pruugi pärast selle aja möödumist enam saada vastuseid Azure AD Graphi lõpp-punktist.</span><span class="sxs-lookup"><span data-stu-id="8beb4-146">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="8beb4-147">**ADAL migreerimine**</span><span class="sxs-lookup"><span data-stu-id="8beb4-147">**ADAL Migration**</span></span>

<span data-ttu-id="8beb4-148">Soovitame võtta kasutusele [Microsofti autentimisteegi (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), mis sisaldab uusimaid funktsioone ja turbevärskendusi.</span><span class="sxs-lookup"><span data-stu-id="8beb4-148">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="8beb4-149">Kui kasutate Microsoft apps ' i, saate teada, et Microsoft on oma rakenduste migreerimise protsessis MSAL lõpptähtajaks, tagades, et nad saavad kasu MSAL pidevast turbest ja funktsioonide täiustustest.</span><span class="sxs-lookup"><span data-stu-id="8beb4-149">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="8beb4-150">Lugege ADAL-i KKK-d.</span><span class="sxs-lookup"><span data-stu-id="8beb4-150">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="8beb4-151">Lugege lisateavet rakenduste platvormipõhise migreerimise kohta.</span><span class="sxs-lookup"><span data-stu-id="8beb4-151">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="8beb4-152">Kui vajate abi selle mõistmiseks, mida teie rakendused kasutavad ADAL, soovitame teil kõigi rakenduste lähtekoodi üle vaadata ja vajadusel jõuda kõigi tarkvaratoode või rakenduste pakkujatega.</span><span class="sxs-lookup"><span data-stu-id="8beb4-152">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="8beb4-153">Samuti saab Microsofti tugi anda teile nimekirja kõigist neist mitte-Microsofti rakendustest teie rentnikkeskkonnas, mis kasutavad ADAL-i.</span><span class="sxs-lookup"><span data-stu-id="8beb4-153">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="8beb4-154">**AAD Graphi migreerimine**</span><span class="sxs-lookup"><span data-stu-id="8beb4-154">**AAD Graph Migration**</span></span>

<span data-ttu-id="8beb4-155">Rakendusi, mis kasutavad Azure AD Graphi, järgige meie juhiseid [AZURE ad Graphi rakenduste migreerimiseks Microsoft Graphi](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span><span class="sxs-lookup"><span data-stu-id="8beb4-155">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. <span data-ttu-id="8beb4-156">[Meie migreerimise kontroll-loend on hea koht alustamiseks](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="8beb4-156">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span>
2. <span data-ttu-id="8beb4-157">Azure‘i rakenduste registreerimisportaalis näete, millised rakendused kasutavad AAD Graphi.</span><span class="sxs-lookup"><span data-stu-id="8beb4-157">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="8beb4-158">Soovitame teil kõigi rakenduste lähtekood läbi vaadata ja kui vaja, võtta ühendust ISV-de või rakendusepakkujatega.</span><span class="sxs-lookup"><span data-stu-id="8beb4-158">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="8beb4-159">Microsofti tugiteenused võivad teile pakkuda ka teie rentniku kõigi AAD Graphide kasutuse loendit.</span><span class="sxs-lookup"><span data-stu-id="8beb4-159">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="8beb4-160">Rakenduses Microsoft Graph andmetele juurdepääsemiseks peab kasutaja või administraator andma sellele loa andmiseks õiged õigused.</span><span class="sxs-lookup"><span data-stu-id="8beb4-160">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="8beb4-161">[Microsoft Graph permissions References](https://docs.microsoft.com/graph/permissions-reference) loetletakse kõigi Microsoft Graphi API-de põhikomplektiga seotud load.</span><span class="sxs-lookup"><span data-stu-id="8beb4-161">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="8beb4-162">See sisaldab ka juhiseid selle kohta, kuidas kasutada lube.</span><span class="sxs-lookup"><span data-stu-id="8beb4-162">It also provides guidance about how to use the permissions.</span></span>
