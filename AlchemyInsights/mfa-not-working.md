---
title: Probleemid MFA-ga
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755127"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="bfe20-102">Azure MFA probleemid</span><span class="sxs-lookup"><span data-stu-id="bfe20-102">Issues with Azure MFA</span></span>
<span data-ttu-id="bfe20-103">Kui kasutajad ei saa mitme teguri autentimise (MFA) abil sisse logida, on mitu võimalust.</span><span class="sxs-lookup"><span data-stu-id="bfe20-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="bfe20-104">Mõjutatud kasutaja võib olla blokeeritud Azure Active Directory portaalis.</span><span class="sxs-lookup"><span data-stu-id="bfe20-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="bfe20-105">Kui see on nii, siis keeldutakse selle konkreetse kasutaja autentimise katsetest automaatselt.</span><span class="sxs-lookup"><span data-stu-id="bfe20-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="bfe20-106">Nende blokeeringu tühistamiseks järgige selle artikli juhiseid.</span><span class="sxs-lookup"><span data-stu-id="bfe20-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="bfe20-107">Kui kasutaja blokeeringu tühistamine ei aidanud või kasutaja ei ole blokeeritud, võite proovida lähtestada MFA kasutaja jaoks ja nad lähevad uuesti registreerumise protsessi.</span><span class="sxs-lookup"><span data-stu-id="bfe20-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="bfe20-108">Palun järgige selle artikli juhiseid.</span><span class="sxs-lookup"><span data-stu-id="bfe20-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="bfe20-109">Kui see on esimene kord, kui lubasite MFA ja kasutajad ei saa sisse logida mitte-brauserite klientidele (nt Outlook, skype jne), võib-olla ADAL (Active Directory autentimine teegis) pole teie O365 tellimusel lubatud.</span><span class="sxs-lookup"><span data-stu-id="bfe20-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="bfe20-110">Sellisel juhul peate looma ühenduse Exchange Online PowerShelliga ja käivitama selle cmdlet-käsk:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*</span><span class="sxs-lookup"><span data-stu-id="bfe20-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>