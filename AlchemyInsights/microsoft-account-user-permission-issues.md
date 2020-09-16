---
title: Probleemi tõrkeotsing – kasutajat ei leitud kataloogist
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725403"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="d3fe4-102">Probleemi tõrkeotsing – kasutajat ei leitud kataloogist</span><span class="sxs-lookup"><span data-stu-id="d3fe4-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="d3fe4-103">Kui kasutajad saavad tõrketeate "kasutaja ei leita", proovige uuesti, kui probleemi tüüp on kasutaja, kes pole kataloogis.</span><span class="sxs-lookup"><span data-stu-id="d3fe4-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="d3fe4-104">Probleemi tõrkeotsinguks saab teha järgmisi toiminguid.</span><span class="sxs-lookup"><span data-stu-id="d3fe4-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="d3fe4-105">Veenduge, et e-posti kutse aktsepteeritud konto on sama konto, mida kasutatakse hiljem sisselogimiseks.</span><span class="sxs-lookup"><span data-stu-id="d3fe4-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="d3fe4-106">Veenduge, et kasutaja kasutab sama kontot, et kutse vastu võtta ja saidile sisse logida.</span><span class="sxs-lookup"><span data-stu-id="d3fe4-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="d3fe4-107">Lisateavet leiate teemast Microsofti [konto pseudonüümide haldamine </a> Microsoft 365 sisselogimise haldamiseks](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="d3fe4-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="d3fe4-108">Sirvige iga saidi (te) ga, kus kasutaja tõrketeate saab.</span><span class="sxs-lookup"><span data-stu-id="d3fe4-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="d3fe4-109">Lisage saidi URL-i lõppu "/_layouts/15/People.aspx/membershipgroupid = 0" (jutumärkides).</span><span class="sxs-lookup"><span data-stu-id="d3fe4-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="d3fe4-110">Näide: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="d3fe4-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="d3fe4-111">Valige loendist kasutaja.</span><span class="sxs-lookup"><span data-stu-id="d3fe4-111">Select the user from the list.</span></span>

- <span data-ttu-id="d3fe4-112">Klõpsake lindil nuppu **Eemalda kasutajaõiguste** .</span><span class="sxs-lookup"><span data-stu-id="d3fe4-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="d3fe4-113">Lisage kasutaja tagasi ja saatke kutse uuesti kasutajale.</span><span class="sxs-lookup"><span data-stu-id="d3fe4-113">Add back the User and Resend the invite to the user.</span></span>

