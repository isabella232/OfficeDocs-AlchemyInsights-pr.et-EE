---
title: Ootamatu mitmikautentimine
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ''
ms.custom:
- "1300007"
- "4372"
ms.openlocfilehash: 8a912b32dee23e8c6eae0ad7bc72228d49ceeb92
ms.sourcegitcommit: 4f7ff981bbb3a98663cd164d0a10bb082cdf7ec9
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 03/25/2020
ms.locfileid: "42946652"
---
# <a name="unexpected-multi-factor-authentication"></a><span data-ttu-id="98af6-102">Ootamatu mitmikautentimine</span><span class="sxs-lookup"><span data-stu-id="98af6-102">Unexpected multi-factor authentication</span></span>

<span data-ttu-id="98af6-103">Kui teie rentnik loodi pärast 21. oktoobrit 2019 ja teilt küsitakse ootamatult mitmikautentimist, olete tõenäoliselt oma rentnikus lubanud [turvalisuse vaikesätted](http://aka.ms/securitydefaults).</span><span class="sxs-lookup"><span data-stu-id="98af6-103">If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](http://aka.ms/securitydefaults) enabled in your tenant.</span></span> 

<span data-ttu-id="98af6-104">Turvalisuse vaikesätete haldamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="98af6-104">To Manage security defaults:</span></span>

1. <span data-ttu-id="98af6-105">Logige oma üldadministraatori identimisteabega [halduskeskusse](https://go.microsoft.com/fwlink/p/?linkid=834822) sisse.</span><span class="sxs-lookup"><span data-stu-id="98af6-105">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="98af6-106">Avage [Azure Active Directory atribuudid](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span><span class="sxs-lookup"><span data-stu-id="98af6-106">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="98af6-107">Lehe allosas klõpsake suvandit **Turvalisuse vaikesätete haldamine**.</span><span class="sxs-lookup"><span data-stu-id="98af6-107">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="98af6-108">Turvalisuse vaikesätete lubamiseks klõpsake **Jah** ja turvalisuse vaikesätete keelamiseks klõpsake **Ei**.</span><span class="sxs-lookup"><span data-stu-id="98af6-108">Click **Yes** to enable security defaults and **No** to disable security defaults.</span></span>
