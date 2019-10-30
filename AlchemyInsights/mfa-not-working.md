---
title: Makromajandusliku finantsabi probleemid
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768833"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="faf36-102">Probleemid Azure MFA</span><span class="sxs-lookup"><span data-stu-id="faf36-102">Issues with Azure MFA</span></span>
<span data-ttu-id="faf36-103">On mõned asjad, mida kontrollida, kui kasutajad ei saa sisse logida, kasutades mitme teguriga autentimine (MFA)</span><span class="sxs-lookup"><span data-stu-id="faf36-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="faf36-104">Mõjutatud kasutaja võib blokeerida Azure Active Directory portaalis.</span><span class="sxs-lookup"><span data-stu-id="faf36-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="faf36-105">Kui see on nii, keelatakse autentimise katsed selle konkreetse kasutaja automaatselt.</span><span class="sxs-lookup"><span data-stu-id="faf36-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="faf36-106">Palun järgige käesoleva artikli juhiseid blokeeringu tühistamiseks.</span><span class="sxs-lookup"><span data-stu-id="faf36-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="faf36-107">Kui kasutaja blokeerimine ei aita või kasutaja ei ole blokeeritud võite proovida lähtestada kasutaja MFA ja nad lähevad läbi registreeruda protsessi uuesti.</span><span class="sxs-lookup"><span data-stu-id="faf36-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="faf36-108">Palun järgige käesoleva artikli juhiseid.</span><span class="sxs-lookup"><span data-stu-id="faf36-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="faf36-109">Kui see on esimene kord, kui aktiveerite MFA ja kasutajad ei saa sisse logida mitte-brauserid klientidele nagu Outlook, Skype, jne, võib-olla ADAL (Active Directory autentimine Raamatukogu) on lubatud teie O365 tellimus.</span><span class="sxs-lookup"><span data-stu-id="faf36-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="faf36-110">Sel juhul peate ühendust Exchange Online PowerShelli ja käivitage see cmdlet-käsu:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*</span><span class="sxs-lookup"><span data-stu-id="faf36-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>