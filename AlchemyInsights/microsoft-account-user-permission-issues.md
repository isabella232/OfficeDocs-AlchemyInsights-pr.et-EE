---
title: Probleemi tõrkeotsinguks - kasutajat ei leitud kataloog
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 537b27d06acd17cbb3fe99bcb89e153099e92bb4
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36544859"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="12f9f-102">Probleemi tõrkeotsinguks - kasutajat ei leitud kataloog</span><span class="sxs-lookup"><span data-stu-id="12f9f-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="12f9f-103">Kui kasutajad saavad viga sõnumi "kasutaja ei leitud" kataloog.</span><span class="sxs-lookup"><span data-stu-id="12f9f-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="12f9f-104">Palun proovige uuesti kui probleemi tüübist pole kasutaja kataloogi.</span><span class="sxs-lookup"><span data-stu-id="12f9f-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="12f9f-105">Järgmised sammud lõpule viia abil probleemi tõrkeotsing.</span><span class="sxs-lookup"><span data-stu-id="12f9f-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="12f9f-106">Tagada e-posti kutse vastu võtnud konto on sama konto, mida kasutatakse hiljem sisse logida.</span><span class="sxs-lookup"><span data-stu-id="12f9f-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="12f9f-107">Veenduge, et kasutaja kasutab sama kontot kutse vastu võtma ja logige sisse.</span><span class="sxs-lookup"><span data-stu-id="12f9f-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="12f9f-108">Lisateabe saamiseks vaadake [haldamine oma Microsofti konto pseudonüümid</a> hallata Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="12f9f-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="12f9f-109">Liikuge iga võrkkoordinaadid, kus kasutaja saab viga.</span><span class="sxs-lookup"><span data-stu-id="12f9f-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="12f9f-110">Lisada "/ _layouts/15/people.aspx/membershipgroupid=0" (maksimaalselt jutumärke) saidi URL-i lõppu.</span><span class="sxs-lookup"><span data-stu-id="12f9f-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="12f9f-111">Näide: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="12f9f-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="12f9f-112">Valige loendist kasutaja.</span><span class="sxs-lookup"><span data-stu-id="12f9f-112">Select the user from the list.</span></span>

- <span data-ttu-id="12f9f-113">Klõpsake nuppu **kasutaja õiguste eemaldamine** lindi.</span><span class="sxs-lookup"><span data-stu-id="12f9f-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="12f9f-114">Kasutajat lisada ja saatke kutse kasutajale.</span><span class="sxs-lookup"><span data-stu-id="12f9f-114">Add back the User and Resend the invite to the user.</span></span>

