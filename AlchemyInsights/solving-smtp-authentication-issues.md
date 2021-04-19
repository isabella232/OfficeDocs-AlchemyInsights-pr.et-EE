---
title: SMTP-autentimisega seotud probleemide lahendamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826411"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="292d2-102">SMTP-autentimisega seotud probleemide lahendamine</span><span class="sxs-lookup"><span data-stu-id="292d2-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="292d2-103">Kui saate SMTP-meili saatmisel ja kliendi või rakendusega autentimisel tõrkeid 5.7.57 või 5.7.3, peaksite kontrollima järgmist.</span><span class="sxs-lookup"><span data-stu-id="292d2-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="292d2-104">Autenditud SMTP-edastus võib olla teie rentnikus või postkastis, mida proovite kasutada(kontrollige mõlemaid sätteid).</span><span class="sxs-lookup"><span data-stu-id="292d2-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="292d2-105">Lisateavet leiate teemast [Autenditud kliendi SMTP-edastuse lubamine või keelamine.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)</span><span class="sxs-lookup"><span data-stu-id="292d2-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="292d2-106">Kontrollige, [kas teie rentniku jaoks on](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) lubatud Azure'i turbe vaikesätted; kui see on lubatud, nurjub SMTP-autentimine põhiautentimise (ehk pärandi; see kasutab kasutajanime ja parooli) kasutamisel.</span><span class="sxs-lookup"><span data-stu-id="292d2-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
