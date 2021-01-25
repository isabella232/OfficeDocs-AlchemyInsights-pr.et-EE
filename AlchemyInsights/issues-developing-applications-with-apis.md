---
title: API-de rakenduste arendamisega seotud probleemid
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974381"
---
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="8a448-102">API-de rakenduste arendamisega seotud probleemid</span><span class="sxs-lookup"><span data-stu-id="8a448-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="8a448-103">Azure Active Directory graafiku API kasutamise alustamiseks lugege artiklit [AZURE ad Graph API Kiirjuhend juhend](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) või vaadake [interaktiivset AZURE ad Graph API dokumentatsiooni](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span><span class="sxs-lookup"><span data-stu-id="8a448-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="8a448-104">**Azure Active Directory autentimise teegi (ADAL) ja Azure AD Graphi API (AAD Graph) toe lõppemine**</span><span class="sxs-lookup"><span data-stu-id="8a448-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="8a448-105">**Alates 30 juunist 2020** ei lisa me enam ADAL ja Azure AD Graphi uusi funktsioone.</span><span class="sxs-lookup"><span data-stu-id="8a448-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="8a448-106">Jätkame tehnilise toe ja turvavärskenduste esitamist, kuid ei paku enam funktsioonide värskendusi.</span><span class="sxs-lookup"><span data-stu-id="8a448-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="8a448-107">**Alates 30 juuni 2022**, lõpetame ADAL ja Azure AD Graphi toe ning ei paku enam tehnilist tuge ega turvavärskendusi.</span><span class="sxs-lookup"><span data-stu-id="8a448-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="8a448-108">Rakendused, mis kasutavad ADAL olemasolevatel OPERATSIOONISÜSTEEMI versioonidel, jätkavad tööd ka pärast seda, kuid ei saa tehnilist tuge ega turvavärskendusi.</span><span class="sxs-lookup"><span data-stu-id="8a448-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="8a448-109">Azure AD Graphi rakendused ei pruugi pärast selle aja möödumist enam saada vastuseid Azure AD Graphi lõpp-punktist.</span><span class="sxs-lookup"><span data-stu-id="8a448-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="8a448-110">**ADAL migreerimine**</span><span class="sxs-lookup"><span data-stu-id="8a448-110">**ADAL Migration**</span></span>

<span data-ttu-id="8a448-111">Soovitame värskendada [Microsoft Authenticationi teeki (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), millel on uusimad funktsioonid ja turvavärskendused.</span><span class="sxs-lookup"><span data-stu-id="8a448-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="8a448-112">Kui kasutate Microsoft apps ' i, saate teada, et Microsoft on oma rakenduste migreerimise protsessis MSAL lõpptähtajaks, tagades, et nad saavad kasu MSAL pidevast turbest ja funktsioonide täiustustest.</span><span class="sxs-lookup"><span data-stu-id="8a448-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="8a448-113">[Lugege ADAL KKK-sid](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="8a448-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="8a448-114">[Siit saate teada, kuidas rakendusi ühe platvormi põhjal migreerida](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="8a448-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="8a448-115">Kui vajate abi selle mõistmiseks, mida teie rakendused kasutavad ADAL, soovitame teil kõigi rakenduste lähtekoodi üle vaadata ja vajadusel jõuda kõigi tarkvaratoode või rakenduste pakkujatega.</span><span class="sxs-lookup"><span data-stu-id="8a448-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="8a448-116">Microsofti tugiteenused võivad anda teile ka kõigi teie rentniku jaoks mitte-Microsofti ADAL rakenduste loendi.</span><span class="sxs-lookup"><span data-stu-id="8a448-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="8a448-117">**AAD Graphi migreerimine**</span><span class="sxs-lookup"><span data-stu-id="8a448-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="8a448-118">Rakendusi, mis kasutavad Azure AD Graphi, järgige meie juhiseid [AZURE ad Graphi rakenduste migreerimiseks Microsoft Graphi](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="8a448-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="8a448-119">[Meie migreerimise kontroll-loend on](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)alustamine.</span><span class="sxs-lookup"><span data-stu-id="8a448-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="8a448-120">Teie Azure ' i rakenduse registreerimise portaal näitab, millised rakendused kasutavad AAD graafikut.</span><span class="sxs-lookup"><span data-stu-id="8a448-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="8a448-121">Soovitame üle vaadata kõik rakenduste lähtekoodi ja vajaduse korral jõuda mõnele tarkvaratoode või rakenduste pakkujale.</span><span class="sxs-lookup"><span data-stu-id="8a448-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="8a448-122">Microsofti tugiteenused võivad teile pakkuda ka teie rentniku kõigi AAD Graphide kasutuse loendit.</span><span class="sxs-lookup"><span data-stu-id="8a448-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="8a448-123">Rakenduses Microsoft Graph andmetele juurdepääsemiseks peab kasutaja või administraator andma sellele loa andmiseks õiged õigused.</span><span class="sxs-lookup"><span data-stu-id="8a448-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="8a448-124">[Microsoft Graph permissions References](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) loetletakse kõigi Microsoft Graphi API-de põhikomplektiga seotud load.</span><span class="sxs-lookup"><span data-stu-id="8a448-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="8a448-125">See sisaldab ka juhiseid selle kohta, kuidas kasutada lube.</span><span class="sxs-lookup"><span data-stu-id="8a448-125">It also provides guidance about how to use the permissions.</span></span>
