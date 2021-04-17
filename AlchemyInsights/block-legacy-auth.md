---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820174"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="3e459-102">Pärandautentimise blokeerimine</span><span class="sxs-lookup"><span data-stu-id="3e459-102">Blocking legacy authentication</span></span>

<span data-ttu-id="3e459-103">Pärandautentimine on termin, mis viitab autentimistaotlusele, mille on teinud:</span><span class="sxs-lookup"><span data-stu-id="3e459-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="3e459-104">Vanemad Office'i kliendid, mis ei kasuta modernautentimist (nt Office 2010 klientrakendus).</span><span class="sxs-lookup"><span data-stu-id="3e459-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="3e459-105">Mis tahes klientrakendus, mis kasutab pärandmeiliprotokolle (nt IMAP/SMTP/POP3).</span><span class="sxs-lookup"><span data-stu-id="3e459-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="3e459-106">Lisateavet pärandautentimise blokeerimise ja modernautentimise lubamise kohta leiate teemast [Pärandautentimise blokeerimine.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)</span><span class="sxs-lookup"><span data-stu-id="3e459-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="3e459-107">Azure Active Directory (Azure AD) turbe vaikesätted hõlbustavad turvalisust ja aitavad kaitsta teie ettevõtet.</span><span class="sxs-lookup"><span data-stu-id="3e459-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="3e459-108">Turbe vaikesätted sisaldavad levinud rünnakute eelkonfigureeritud turbesätteid.</span><span class="sxs-lookup"><span data-stu-id="3e459-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="3e459-109">Lisateavet turbe vaikesätete kohta leiate teemast Mis [on turbe vaikesätted?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="3e459-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="3e459-110">**Märkus.** Kui teie rentnik loodi 22. oktoobril 2019 või pärast seda, on võimalik, et teil on uus turvaline vaikekäitumine ja teie rentnikus on turbe vaikesätted juba lubatud.</span><span class="sxs-lookup"><span data-stu-id="3e459-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="3e459-111">Selleks et kaitsta kõiki meie kasutajaid, tehakse turbe vaikesätted kõigile loodud rentnikele.</span><span class="sxs-lookup"><span data-stu-id="3e459-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
