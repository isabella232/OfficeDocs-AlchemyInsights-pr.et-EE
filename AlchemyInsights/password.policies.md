---
title: Parooli reeglid
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743956"
---
# <a name="password-policies"></a><span data-ttu-id="8a4cc-102">Parooli reeglid</span><span class="sxs-lookup"><span data-stu-id="8a4cc-102">Password policies</span></span>

<span data-ttu-id="8a4cc-103">**Mul on probleeme kasutaja parooli poliitikaga**</span><span class="sxs-lookup"><span data-stu-id="8a4cc-103">**I'm having problems with the password policy for a user**</span></span>

- <span data-ttu-id="8a4cc-104">Kasutaja paroolide poliitika sõltub sellest, kas kasutaja on ainult pilves või kohapealne.</span><span class="sxs-lookup"><span data-stu-id="8a4cc-104">The password policy for a user depends on whether the user is cloud only or on-premises.</span></span>
- <span data-ttu-id="8a4cc-105">Ainult pilveteenuse kasutajad peavad valima parooli, mis vastab selle artikli nõuetele: [paroolide poliitika, mis rakenduvad ainult pilveteenuse kasutajakontodele](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="8a4cc-105">Cloud only users must choose a password that meets the requirements in this article: [Password policies that only apply to cloud user accounts](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span></span>
- <span data-ttu-id="8a4cc-106">Kohapealsetel kasutajatel tuleb valida parool, mis vastab kohapealsetele nõuetele.</span><span class="sxs-lookup"><span data-stu-id="8a4cc-106">On-premises users must choose a password that meets the on-premises requirements.</span></span> <span data-ttu-id="8a4cc-107">Kui kohapealne kasutaja ei saa oma parooli määrata, kontrollige kohapealseid nõudeid.</span><span class="sxs-lookup"><span data-stu-id="8a4cc-107">If an on-premises user is unable to set their password, check your on-premises requirements.</span></span>

<span data-ttu-id="8a4cc-108">**Ma ei tea, kuidas parooli aegumise poliitikaid määrata või kontrollida**</span><span class="sxs-lookup"><span data-stu-id="8a4cc-108">**I don't know how to set or check password expiration policies**</span></span>

- <span data-ttu-id="8a4cc-109">Saate määrata ja kontrollida oma rentniku jaoks mõeldud pilve kasutajate aegumise poliitikat PowerShelli abil.</span><span class="sxs-lookup"><span data-stu-id="8a4cc-109">You can set and check the expiration policy for cloud users in your tenant by using PowerShell.</span></span> <span data-ttu-id="8a4cc-110">Järgige selle artikli juhiseid: [paroolide määramine või kontrollimine PowerShelli abil](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span><span class="sxs-lookup"><span data-stu-id="8a4cc-110">Follow the instructions in this article: [Set or check the password policies by using PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span></span>
- <span data-ttu-id="8a4cc-111">Kohapealsete kasutajate parooli aegumise poliitika määratakse teie kohapealses REKLAAMIs.</span><span class="sxs-lookup"><span data-stu-id="8a4cc-111">The password expiration policy for on-premises users is set in your on-premises AD.</span></span>

<span data-ttu-id="8a4cc-112">**Muud kasulikud lingid.**</span><span class="sxs-lookup"><span data-stu-id="8a4cc-112">**Other Helpful links:**</span></span>
- [<span data-ttu-id="8a4cc-113">Paroolilähtestusketta kasutamise alustamine</span><span class="sxs-lookup"><span data-stu-id="8a4cc-113">Getting Started with Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [<span data-ttu-id="8a4cc-114">Administraatori algatatud parooli lähtestamise tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="8a4cc-114">Troubleshoot Administrator-initiated Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
