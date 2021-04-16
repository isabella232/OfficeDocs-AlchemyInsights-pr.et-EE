---
title: Probleemid MFA-ga
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810480"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="a739c-102">Azure'i MFA probleemid</span><span class="sxs-lookup"><span data-stu-id="a739c-102">Issues with Azure MFA</span></span>
<span data-ttu-id="a739c-103">On paar asja, mida kontrollida, kas kasutajad ei saa mitme teguriga autentimise (MFA) abil sisse logida</span><span class="sxs-lookup"><span data-stu-id="a739c-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="a739c-104">Mõjutatud kasutaja võib olla Azure Active Directory portaalis blokeeritud.</span><span class="sxs-lookup"><span data-stu-id="a739c-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="a739c-105">Sel juhul keelatakse selle konkreetse kasutaja autentimiskatsed automaatselt.</span><span class="sxs-lookup"><span data-stu-id="a739c-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="a739c-106">Nende blokeeringu tühistamiseks järgige selles artiklis toodud juhiseid.</span><span class="sxs-lookup"><span data-stu-id="a739c-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="a739c-107">Kui kasutaja blokeeringu tühistamisest polnud abi või kasutaja pole blokeeritud, võite proovida kasutaja jaoks MFA lähtestada ja ta läbib registreerumise uuesti.</span><span class="sxs-lookup"><span data-stu-id="a739c-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="a739c-108">Järgige selles artiklis toodud juhiseid.</span><span class="sxs-lookup"><span data-stu-id="a739c-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="a739c-109">Kui lubate MFA esimest korda ja teie kasutajad ei saa sisse logida brauserivälistesse klientrakendusse (nt Outlook, Skype jne), siis võib-olla pole teie O365 tellimuses lubatud ADAL (Active Directory autentimisteek).</span><span class="sxs-lookup"><span data-stu-id="a739c-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="a739c-110">Sel juhul peate exchange Online'i PowerShelliga ühenduse loomiseks ja käivitama selle  *cmdlet-käsu: Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="a739c-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>