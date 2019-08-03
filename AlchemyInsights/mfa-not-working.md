---
title: Probleemid makromajandusliku finantsabi
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
ms.openlocfilehash: 2e79040c249b7825b964a19c51bcc42e5a6afb3f
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/26/2019
ms.locfileid: "35250161"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="13c95-102">Probleemid makromajandusliku finantsabi</span><span class="sxs-lookup"><span data-stu-id="13c95-102">Issues with MFA</span></span>
<span data-ttu-id="13c95-103">On paar asja kontrollida, kui kasutajad ei saa sisse logida, kasutades mitme teguriga autentimine (MFA)</span><span class="sxs-lookup"><span data-stu-id="13c95-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="13c95-104">Mõjutatud kasutaja võib blokeerida Azure Active Directory keskkonnas.</span><span class="sxs-lookup"><span data-stu-id="13c95-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="13c95-105">Kui see juhtub, autentimise katsed selleks keelatakse automaatselt konkreetse kasutaja.</span><span class="sxs-lookup"><span data-stu-id="13c95-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="13c95-106">Palun järgige selles artiklis endi blokeerimise lõpetamist.</span><span class="sxs-lookup"><span data-stu-id="13c95-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="13c95-107">Kui kasutaja on blokeeritud või blokeeringu kasutaja ei aidanud proovige lähtestada kasutaja MFA ja nad lähevad läbi registreeruda protsessi uuesti.</span><span class="sxs-lookup"><span data-stu-id="13c95-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="13c95-108">Palun järgige selles artiklis.</span><span class="sxs-lookup"><span data-stu-id="13c95-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="13c95-109">Kui esimest korda te lubatud MFA ja kasutajad ei saa logida-brauserid kliendid, nagu Outlook, Skype jne, ehk ADAL (Active Directory autentimise Raamatukogu) on sisse lülitatud tellimuse O365.</span><span class="sxs-lookup"><span data-stu-id="13c95-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="13c95-110">Sel juhul peate ühendust Exchange Online PowerShelli ja käivitada:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="13c95-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>