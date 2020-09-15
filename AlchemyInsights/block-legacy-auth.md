---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685594"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="3b6b1-102">Pärandi autentimise blokeerimine</span><span class="sxs-lookup"><span data-stu-id="3b6b1-102">Blocking legacy authentication</span></span>

<span data-ttu-id="3b6b1-103">Pärand autentimine on termin, mis viitab autentimise taotlusele, mille on teinud:</span><span class="sxs-lookup"><span data-stu-id="3b6b1-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="3b6b1-104">Vanemad Office ' i kliendid, kes ei kasuta tänapäevast autentimist (nt Office 2010 Client).</span><span class="sxs-lookup"><span data-stu-id="3b6b1-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="3b6b1-105">Iga klient, kes kasutab pärand mail Protocols (nt IMAP/SMTP/POP3).</span><span class="sxs-lookup"><span data-stu-id="3b6b1-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="3b6b1-106">Lisateavet pärandi autentimise blokeerimise ja kaasaegse autentimise lubamise kohta leiate teemast [pärandi autentimise blokeerimine](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="3b6b1-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="3b6b1-107">Azure Active Directory (Azure AD) turbe vaikesätted hõlbustavad turvalisust ja aitavad kaitsta teie ettevõtet.</span><span class="sxs-lookup"><span data-stu-id="3b6b1-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="3b6b1-108">Turbe vaikeväärtused sisaldavad levinumate rünnakute eelkonfigureeritud turvasätteid.</span><span class="sxs-lookup"><span data-stu-id="3b6b1-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="3b6b1-109">Lisateavet turbe vaikesätete kohta leiate teemast [mis on turbe vaikesätted?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="3b6b1-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="3b6b1-110">**Märkus**: kui teie rentnik oli loodud 22 oktoobril, 2019, on võimalik, et teil esineb uus turva-ja vaike-käitumine ning teil on juba rentniku jaoks lubatud turvalisus.</span><span class="sxs-lookup"><span data-stu-id="3b6b1-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="3b6b1-111">Kõigi kasutajate kaitsmiseks rullitakse turbe vaikeväärtused kõigi uute rentnike jaoks loodud uute rentnike jaoks.</span><span class="sxs-lookup"><span data-stu-id="3b6b1-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
