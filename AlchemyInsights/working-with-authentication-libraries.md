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
# <a name="working-with-authentication-libraries"></a><span data-ttu-id="d991f-102">Autentimine teekidega töötamine</span><span class="sxs-lookup"><span data-stu-id="d991f-102">Working with Authentication Libraries</span></span>

<span data-ttu-id="d991f-103">Microsofti autentimise teegi (MSAL) probleemi lahendamiseks tehke järgmist soovitatud toiminguid.</span><span class="sxs-lookup"><span data-stu-id="d991f-103">To resolve Microsoft Authentication Library (MSAL) issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="d991f-104">**Töötamine MSAL**: [Microsofti identiteedi platvormi autentimine teegid](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) – selles artiklis kirjeldatakse mitme rakenduse tüüpi Microsofti autentimise teegi tuge.</span><span class="sxs-lookup"><span data-stu-id="d991f-104">**Working with MSAL**: [Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - This article shows Microsoft Authentication Library support for several application types.</span></span> <span data-ttu-id="d991f-105">See sisaldab linke teegi lähtekoodi; kust saada oma rakenduse projekti pakett; ja kas teek toetab kasutaja sisselogimist (autentimine), juurdepääsu kaitstud Web API-de (autoriseerimine) või mõlemat.</span><span class="sxs-lookup"><span data-stu-id="d991f-105">It includes links to library source code; where to get the package for your app's project; and whether the library supports user sign-in (authentication), access to protected web APIs (authorization), or both.</span></span>

2. <span data-ttu-id="d991f-106">**Autentimise tõrkeotsing**: MSAL toetab mitmeid autentimise voogusid eri rakenduse stsenaariumite jaoks.</span><span class="sxs-lookup"><span data-stu-id="d991f-106">**Troubleshoot Authentication**: The MSAL supports several authentication flows for use in different application scenarios.</span></span> <span data-ttu-id="d991f-107">Olenevalt sellest, kuidas teie klientrakendus on loodud, saab MSAL kasutada ühte või mitut Microsofti identiteedi platvormi toetatud autentimise voogusid.</span><span class="sxs-lookup"><span data-stu-id="d991f-107">Depending on how your client application is built, the MSAL can use one or more of the authentication flows supported by the Microsoft identity platform.</span></span> <span data-ttu-id="d991f-108">Need vood võivad toota mitut tüüpi lube ja autoriseerimise koode ning nõuda nende töö tegemiseks erinevaid märke.</span><span class="sxs-lookup"><span data-stu-id="d991f-108">These flows can produce several types of tokens and authorization codes, and require different tokens to make them work.</span></span>

3. <span data-ttu-id="d991f-109">**Accessi märgid**: [Microsoft Identity Platform Accessi märked](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – saate teada, kuidas teie API saab kinnitada ja kasutada Accessi loaga olevaid nõudeid.</span><span class="sxs-lookup"><span data-stu-id="d991f-109">**Access Tokens**: [Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Learn how your API can validate and use the claims inside an access token.</span></span> <span data-ttu-id="d991f-110">Kõik selle artikli dokumendid, välja arvatud juhul, kui need on märgitud, rakenduvad ainult registreeritud API-de jaoks väljaantud märkide korral.</span><span class="sxs-lookup"><span data-stu-id="d991f-110">All documentation in this article, except where noted, applies only to tokens issued for APIs you've registered.</span></span> <span data-ttu-id="d991f-111">Seda ei kohaldata Microsofti omanduses olevate API-de jaoks välja antud märkide suhtes, samuti ei saa neid märke kasutada selleks, et valideerida, kuidas Microsoft Identity Platform teie loodud API jaoks lube väljastab.</span><span class="sxs-lookup"><span data-stu-id="d991f-111">It does not apply to tokens issued for Microsoft-owned APIs, nor can those tokens be used to validate how the Microsoft identity platform will issue tokens for an API you create.</span></span>

<span data-ttu-id="d991f-112">**Azure Active Directory autentimise teegi (ADAL) toe lõpp**</span><span class="sxs-lookup"><span data-stu-id="d991f-112">**End of support for Azure Active Directory Authentication Library (ADAL)**</span></span>

- <span data-ttu-id="d991f-113">**Alates 30 juunist 2020** ei lisa me enam ADAL ja Azure AD Graphi uusi funktsioone.</span><span class="sxs-lookup"><span data-stu-id="d991f-113">**Starting June 30th, 2020,** we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="d991f-114">Pakume endiselt tehnilist tuge ja turbevärskendusi, ent mitte enam funktsioonivärskendusi.</span><span class="sxs-lookup"><span data-stu-id="d991f-114">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
- <span data-ttu-id="d991f-115">**Alates 30 juuni 2022,** lõpetame ADAL ja Azure AD Graphi toe ning ei paku enam tehnilist tuge ega turvavärskendusi.</span><span class="sxs-lookup"><span data-stu-id="d991f-115">**Starting June 30th, 2022,** we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>
- <span data-ttu-id="d991f-116">Rakendused, mis kasutavad ADAL olemasolevatel OPERATSIOONISÜSTEEMI versioonidel, jätkavad tööd ka pärast seda, kuid ei *saa tehnilist tuge ega turvavärskendusi*.</span><span class="sxs-lookup"><span data-stu-id="d991f-116">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>
- <span data-ttu-id="d991f-117">Azure AD Graphi rakendused ei pruugi pärast selle aja möödumist enam saada vastuseid Azure AD Graphi lõpp-punktist.</span><span class="sxs-lookup"><span data-stu-id="d991f-117">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="d991f-118">**ADAL migreerimine**</span><span class="sxs-lookup"><span data-stu-id="d991f-118">**ADAL Migration**</span></span>

- <span data-ttu-id="d991f-119">Soovitame värskendada MSAL, millel on uusimad funktsioonid ja turvavärskendused.</span><span class="sxs-lookup"><span data-stu-id="d991f-119">We recommend updating to the MSAL, which has the latest features and security updates.</span></span>
- <span data-ttu-id="d991f-120">Kui kasutate Microsoft apps ' i, saate teada, et Microsoft on oma rakenduste migreerimise protsessis MSAL lõpptähtajaks, tagades, et nad saavad kasu MSAL pidevast turbest ja funktsioonide täiustustest.</span><span class="sxs-lookup"><span data-stu-id="d991f-120">If you're using Microsoft apps, know that Microsoft is in the process of migrating its apps to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="d991f-121">[Lugege ADAL KKK-sid](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="d991f-121">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
2. <span data-ttu-id="d991f-122">[Siit saate teada, kuidas rakendusi ühe platvormi põhjal migreerida](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span><span class="sxs-lookup"><span data-stu-id="d991f-122">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span></span>
3. <span data-ttu-id="d991f-123">Kui teil on pärast rakenduse platvormile lisatud juhendi lugemist lisaküsimusi, saate postitada [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) sildiga [Azure-AD-ADAL-aegunud] või avada probleemi teegi github hoidlas.</span><span class="sxs-lookup"><span data-stu-id="d991f-123">If, after reading the guide for your app's platform, you have additional questions, you can post on [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) with the tag [azure-ad-adal-deprecation] or open an issue in library's GitHub repository.</span></span> <span data-ttu-id="d991f-124">Iga teegi Repo lingid leiate teemast **MSAL ülevaade** artiklist [keeled ja raamistikud](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) .</span><span class="sxs-lookup"><span data-stu-id="d991f-124">See the [Languages and frameworks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) section of the **MSAL overview** article for links to each library's repo.</span></span>
4. <span data-ttu-id="d991f-125">**Kui vajate abi selle kohta, millised rakendused kasutavad ADAL**, soovitame teil kõik oma rakenduste lähtekoodi üle vaadata.</span><span class="sxs-lookup"><span data-stu-id="d991f-125">**If you need help understanding which of your apps use ADAL**, we recommend you review all of your apps' source code.</span></span> <span data-ttu-id="d991f-126">Vajadusel REACH-iga sõltumatute tarkvara tarnijate (tarkvaratoode) või rakenduste pakkujatega.</span><span class="sxs-lookup"><span data-stu-id="d991f-126">If applicable, reach out to any Independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="d991f-127">Samuti saab Microsofti tugi anda teile nimekirja kõigist neist mitte-Microsofti rakendustest teie rentnikkeskkonnas, mis kasutavad ADAL-i.</span><span class="sxs-lookup"><span data-stu-id="d991f-127">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>







