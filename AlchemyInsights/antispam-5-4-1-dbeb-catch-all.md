---
title: Rämpspostitõrje 5.4.1 DBEB saagi-kõik
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707907"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="fa5b1-102">Fix kohaletoimetamise probleemid tõrkekood 550 5.4.1 relee juurdepääs keelatud</span><span class="sxs-lookup"><span data-stu-id="fa5b1-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="fa5b1-103">See probleem ilmneb siis [, kui kontrollida, kas e-posti aadress on kehtiv vältida bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) sisestamisel Microsoft Network.</span><span class="sxs-lookup"><span data-stu-id="fa5b1-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="fa5b1-104">Proovige järgmist:</span><span class="sxs-lookup"><span data-stu-id="fa5b1-104">Try the following:</span></span>

1. <span data-ttu-id="fa5b1-105">Tehke kindlaks, kas probleem on seotud kogu domeeni või ühe e-posti aadress:</span><span class="sxs-lookup"><span data-stu-id="fa5b1-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="fa5b1-106">Kogu Domeen: mõnikord peab Domeen olema sünkroonitud; Proovige [domeeni sisemine ja seejärel tagasi autoriteetne](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="fa5b1-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="fa5b1-107">Üks e-posti aadress: mõnikord tuleb aadress sünkroonida; SMTP puhverserveri aadressi muutmine ja seejärel uuesti muutmine aitab.</span><span class="sxs-lookup"><span data-stu-id="fa5b1-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="fa5b1-108">Tehke kindlaks, kas probleem on seotud rühma või ühiskausta.</span><span class="sxs-lookup"><span data-stu-id="fa5b1-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="fa5b1-109">Mõne objektitüübi puhul võib osutuda vajalikuks objektide käsitsi loomine Azure Active Directorys.</span><span class="sxs-lookup"><span data-stu-id="fa5b1-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="fa5b1-110">Kui vajate täiendavat abi, siis avage tugiteenuse pilet ja määrake probleemi ulatus (sh teie poolt saatva objekti tüüp), et saaksime teid paremini aidata.</span><span class="sxs-lookup"><span data-stu-id="fa5b1-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>