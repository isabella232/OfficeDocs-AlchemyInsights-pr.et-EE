---
title: Rakenduste väljatöötamise probleemid
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974304"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="dc091-102">Rakenduste väljatöötamise probleemid</span><span class="sxs-lookup"><span data-stu-id="dc091-102">Issues developing applications</span></span>

<span data-ttu-id="dc091-103">Azure Active Directory (AD) rakenduste loomisel kõige levinumate probleemide tõrkeotsinguks lugege järgmisi artikleid.</span><span class="sxs-lookup"><span data-stu-id="dc091-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="dc091-104">Näen probleeme ainult Chrome ' i brauseri kaudu sisselogimisel rakendusse (desse)</span><span class="sxs-lookup"><span data-stu-id="dc091-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="dc091-105">Ma ei tea, kuidas muuta rakenduse turbelubade kasutuse vaikesätteid</span><span class="sxs-lookup"><span data-stu-id="dc091-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="dc091-106">Olen segaduses selle pärast, kuidas rakenduse nõusolek töötab</span><span class="sxs-lookup"><span data-stu-id="dc091-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="dc091-107">Ma ei tea, kuidas oma rakendusele lube anda</span><span class="sxs-lookup"><span data-stu-id="dc091-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="dc091-108">Ma ei saa aru delegeeritud ja rakenduse kasutusõiguste erinevusest</span><span class="sxs-lookup"><span data-stu-id="dc091-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="dc091-109">\***Azure Active Directory autentimise teegi (ADAL) ja AZURE ad Graph API (AAD Graph) _ toe lõppemine**</span><span class="sxs-lookup"><span data-stu-id="dc091-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="dc091-110">Alates 30 juunist 2020 ei lisa me enam Azure Active Directory autentimise teeki (ADAL) ja Azure AD Graph API-d (AAD Graph) uusi funktsioone.</span><span class="sxs-lookup"><span data-stu-id="dc091-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="dc091-111">Jätkame tehnilise toe ja turvavärskenduste esitamist, kuid ei paku enam funktsioonide värskendusi.</span><span class="sxs-lookup"><span data-stu-id="dc091-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="dc091-112">Alates 30 juunist 2022, lõpetame ADAL ja AAD graafiku toe ning ei paku enam tehnilist tuge ega turvavärskendusi.</span><span class="sxs-lookup"><span data-stu-id="dc091-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="dc091-113">Selle tingimuse tulemusena on järgmised tagajärjed.</span><span class="sxs-lookup"><span data-stu-id="dc091-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="dc091-114">Rakendused, mis kasutavad ADAL olemasolevatel OPERATSIOONISÜSTEEMI versioonidel, jätkavad tööd ka pärast seda, kuid ei saa tehnilist tuge ega turvavärskendusi.</span><span class="sxs-lookup"><span data-stu-id="dc091-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="dc091-115">Rakendused, mis kasutavad AAD Graph ' i, ei pruugi enam saada vastuseid AAD Graph Endpoint</span><span class="sxs-lookup"><span data-stu-id="dc091-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="dc091-116">_ *ADAL migreerimine*\*</span><span class="sxs-lookup"><span data-stu-id="dc091-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="dc091-117">Kui kasutate Microsofti rakendusi, soovitame värskendada Microsoft Authenticationi teeki (MSAL), kus on uusimad funktsioonid ja turvavärskendused.</span><span class="sxs-lookup"><span data-stu-id="dc091-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="dc091-118">See soovitus on Microsofti kontekstis, mille käigus alustatakse selle rakenduste migreerimist MSAL lõpptähtpäeva järgi.</span><span class="sxs-lookup"><span data-stu-id="dc091-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="dc091-119">Microsoft oma rakenduste migreerimine MSAL tagab, et rakendused saavad kasu MSAL pidevast turbest ja funktsioonide täiustustest.</span><span class="sxs-lookup"><span data-stu-id="dc091-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="dc091-120">Lugege ADAL KKK-sid</span><span class="sxs-lookup"><span data-stu-id="dc091-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="dc091-121">Vaadake, kuidas rakendusi ühe platvormi põhjal migreerida</span><span class="sxs-lookup"><span data-stu-id="dc091-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="dc091-122">Kui vajate abi selle mõistmisel, mida teie rakendused kasutavad ADAL, soovitame teil kõigi rakenduste lähtekoodi üle vaadata ja vajaduse korral jõuda kõigi sõltumatute tarkvara tarnijate (tarkvaratoode) või rakenduste pakkujatega.</span><span class="sxs-lookup"><span data-stu-id="dc091-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="dc091-123">Microsofti tugiteenused võivad anda teile ka kõigi teie rentniku jaoks mitte-Microsofti ADAL rakenduste loendi.</span><span class="sxs-lookup"><span data-stu-id="dc091-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="dc091-124">**AAD Graphi migreerimine**</span><span class="sxs-lookup"><span data-stu-id="dc091-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="dc091-125">Kui teil on rakenduses AAD Graph kasutatavaid rakendusi, järgige meie juhiseid AAD Graph ' i rakenduste migreerimiseks Microsoft Graphi.</span><span class="sxs-lookup"><span data-stu-id="dc091-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="dc091-126">[Meie migreerimise kontroll-loend on](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)alustamine.</span><span class="sxs-lookup"><span data-stu-id="dc091-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="dc091-127">Teie Azure ' i rakenduse registreerimise portaal näitab, millised rakendused kasutavad AAD graafikut.</span><span class="sxs-lookup"><span data-stu-id="dc091-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="dc091-128">Soovitame üle vaadata kõik rakenduste lähtekoodi ja vajaduse korral jõuda iseseisvate tarkvara tarnijate (tarkvaratoode) või rakenduste pakkujatega.</span><span class="sxs-lookup"><span data-stu-id="dc091-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="dc091-129">Microsofti tugiteenused võivad anda teile teavet ka teie rentniku AAD Graphi kasutamise kohta.</span><span class="sxs-lookup"><span data-stu-id="dc091-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







