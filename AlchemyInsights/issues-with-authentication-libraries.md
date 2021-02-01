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
# <a name="issues-with-authentication-libraries"></a><span data-ttu-id="ae480-102">Autentimise teekidega seotud probleemid</span><span class="sxs-lookup"><span data-stu-id="ae480-102">Issues with Authentication Libraries</span></span>

1. <span data-ttu-id="ae480-103">[Microsofti identiteedi platvormi autentimise teegid](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) on loetletud Microsoft-toetatud ja ühilduvad kliendi ja vahevarade teegid</span><span class="sxs-lookup"><span data-stu-id="ae480-103">[Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lists Microsoft-supported and compatible client and middleware libraries.</span></span>
2. <span data-ttu-id="ae480-104">Microsofti autentimise teek (MSAL) toetab mitmeid [autentimise voogusid](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) eri rakenduse stsenaariumite jaoks.</span><span class="sxs-lookup"><span data-stu-id="ae480-104">The Microsoft Authentication Library (MSAL) supports several [authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for use in different application scenarios.</span></span>
3. <span data-ttu-id="ae480-105">Märkide autentimiseks ja hankimiseks lähtestage oma koodis uus avalik või konfidentsiaalne klientrakendus.</span><span class="sxs-lookup"><span data-stu-id="ae480-105">To authenticate and acquire tokens, you initialize a new public or confidential client application in your code.</span></span> <span data-ttu-id="ae480-106">Saate määrata mitu seadistusvõimalusi, kui käivitate Microsofti autentimise teegis (MSAL) klientrakenduse rakenduse.</span><span class="sxs-lookup"><span data-stu-id="ae480-106">You can set several configuration options when you initialize the client app in the Microsoft Authentication Library (MSAL).</span></span> <span data-ttu-id="ae480-107">Lisateavet leiate teemast [rakenduse konfigureerimise suvandid](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span><span class="sxs-lookup"><span data-stu-id="ae480-107">To learn more, see [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span></span>

<span data-ttu-id="ae480-108">**Azure Active Directory autentimise teegi (ADAL) ja Azure AD Graphi API (AAD Graph) toe lõppemine**</span><span class="sxs-lookup"><span data-stu-id="ae480-108">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="ae480-109">**Alates 30 juunist 2020** ei lisa me enam ADAL ja Azure AD Graphi uusi funktsioone.</span><span class="sxs-lookup"><span data-stu-id="ae480-109">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="ae480-110">Pakume endiselt tehnilist tuge ja turbevärskendusi, ent mitte enam funktsioonivärskendusi.</span><span class="sxs-lookup"><span data-stu-id="ae480-110">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="ae480-111">**Alates 30 juuni 2022**, lõpetame ADAL ja Azure AD Graphi toe ning ei paku enam tehnilist tuge ega turvavärskendusi.</span><span class="sxs-lookup"><span data-stu-id="ae480-111">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="ae480-112">Rakendused, mis kasutavad ADAL olemasolevatel OPERATSIOONISÜSTEEMI versioonidel, jätkavad tööd ka pärast seda, kuid ei *saa tehnilist tuge ega turvavärskendusi*.</span><span class="sxs-lookup"><span data-stu-id="ae480-112">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="ae480-113">Azure AD Graphi rakendused ei pruugi pärast selle aja möödumist enam saada vastuseid Azure AD Graphi lõpp-punktist.</span><span class="sxs-lookup"><span data-stu-id="ae480-113">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="ae480-114">**ADAL migreerimine**</span><span class="sxs-lookup"><span data-stu-id="ae480-114">**ADAL Migration**</span></span>

<span data-ttu-id="ae480-115">Soovitame võtta kasutusele [Microsofti autentimisteegi (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), mis sisaldab uusimaid funktsioone ja turbevärskendusi.</span><span class="sxs-lookup"><span data-stu-id="ae480-115">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="ae480-116">Kui kasutate Microsoft apps ' i, saate teada, et Microsoft on oma rakenduste migreerimise protsessis MSAL lõpptähtpäevaks, tagades, et nad saavad kasu MSAL pidevast turbest ja funktsioonide täiustustest.</span><span class="sxs-lookup"><span data-stu-id="ae480-116">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they will benefit from MSAL's ongoing security and feature improvements.</span></span>

<span data-ttu-id="ae480-117">Lisateavet leiate järgmistest teemadest:</span><span class="sxs-lookup"><span data-stu-id="ae480-117">For more information, see:</span></span>

1. [<span data-ttu-id="ae480-118">Lugege ADAL-i KKK-d.</span><span class="sxs-lookup"><span data-stu-id="ae480-118">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="ae480-119">Lugege lisateavet rakenduste platvormipõhise migreerimise kohta.</span><span class="sxs-lookup"><span data-stu-id="ae480-119">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="ae480-120">Kui vajate abi selle mõistmiseks, mida teie rakendused kasutavad ADAL, soovitame teil kõigi rakenduste lähtekoodi üle vaadata ja vajadusel jõuda kõigi tarkvaratoode või rakenduste pakkujatega.</span><span class="sxs-lookup"><span data-stu-id="ae480-120">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="ae480-121">Samuti saab Microsofti tugi anda teile nimekirja kõigist neist mitte-Microsofti rakendustest teie rentnikkeskkonnas, mis kasutavad ADAL-i.</span><span class="sxs-lookup"><span data-stu-id="ae480-121">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="ae480-122">**AAD Graphi migreerimine**</span><span class="sxs-lookup"><span data-stu-id="ae480-122">**AAD Graph Migration**</span></span>

<span data-ttu-id="ae480-123">Rakendusi, mis kasutavad Azure AD Graphi, järgige meie juhiseid [AZURE ad Graphi rakenduste migreerimiseks Microsoft Graphi](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span><span class="sxs-lookup"><span data-stu-id="ae480-123">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. [<span data-ttu-id="ae480-124">Meie migreerimise kontroll-loend on alustamine.</span><span class="sxs-lookup"><span data-stu-id="ae480-124">Our migration checklist provides a getting started point.</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. <span data-ttu-id="ae480-125">Azure‘i rakenduste registreerimisportaalis näete, millised rakendused kasutavad AAD Graphi.</span><span class="sxs-lookup"><span data-stu-id="ae480-125">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="ae480-126">Soovitame teil kõigi rakenduste lähtekood läbi vaadata ja kui vaja, võtta ühendust ISV-de või rakendusepakkujatega.</span><span class="sxs-lookup"><span data-stu-id="ae480-126">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="ae480-127">Microsofti tugiteenused võivad teile pakkuda ka teie rentniku kõigi AAD Graphide kasutuse loendit.</span><span class="sxs-lookup"><span data-stu-id="ae480-127">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="ae480-128">Rakenduses Microsoft Graph andmetele juurdepääsemiseks peab kasutaja või administraator andma sellele loa andmiseks õiged õigused.</span><span class="sxs-lookup"><span data-stu-id="ae480-128">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="ae480-129">[Microsoft Graph permissions References](https://docs.microsoft.com/graph/permissions-reference) loetletakse kõigi Microsoft Graphi API-de põhikomplektiga seotud load.</span><span class="sxs-lookup"><span data-stu-id="ae480-129">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="ae480-130">See sisaldab ka juhiseid selle kohta, kuidas kasutada lube.</span><span class="sxs-lookup"><span data-stu-id="ae480-130">It also provides guidance about how to use the permissions.</span></span>
