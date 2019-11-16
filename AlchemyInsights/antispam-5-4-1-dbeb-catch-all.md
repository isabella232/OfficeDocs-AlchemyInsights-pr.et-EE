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
ms.openlocfilehash: 4f531a063d63aff239ef7dead869bb526e17fb35
ms.sourcegitcommit: 2591e1f56e8943bddb9d3b77ba5b494ac49d4f30
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 11/15/2019
ms.locfileid: "38672429"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="8ff0b-102">Fix kohaletoimetamise probleemid tõrkekood 550 5.4.1 relee juurdepääs keelatud</span><span class="sxs-lookup"><span data-stu-id="8ff0b-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="8ff0b-103">See probleem ilmneb siis [, kui kontrollida, kas e-posti aadress on kehtiv vältida bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) sisestamisel Office 365 võrgu.</span><span class="sxs-lookup"><span data-stu-id="8ff0b-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Office 365 network.</span></span> <span data-ttu-id="8ff0b-104">Proovige järgmist:</span><span class="sxs-lookup"><span data-stu-id="8ff0b-104">Try the following:</span></span>

1. <span data-ttu-id="8ff0b-105">Tehke kindlaks, kas probleem on seotud kogu domeeni või ühe e-posti aadress:</span><span class="sxs-lookup"><span data-stu-id="8ff0b-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="8ff0b-106">Kogu Domeen: mõnikord peab Domeen olema sünkroonitud; Proovige [domeeni sisemine ja seejärel tagasi autoriteetne](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="8ff0b-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="8ff0b-107">Üks e-posti aadress: mõnikord tuleb aadress sünkroonida; SMTP puhverserveri aadressi muutmine ja seejärel uuesti muutmine aitab.</span><span class="sxs-lookup"><span data-stu-id="8ff0b-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="8ff0b-108">Tehke kindlaks, kas probleem on seotud rühma või ühiskausta.</span><span class="sxs-lookup"><span data-stu-id="8ff0b-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="8ff0b-109">Mõne objektitüübi puhul võib osutuda vajalikuks objektide käsitsi loomine Azure Active Directorys.</span><span class="sxs-lookup"><span data-stu-id="8ff0b-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="8ff0b-110">Kui vajate täiendavat abi, siis avage tugiteenuse pilet ja määrake probleemi ulatus (sh teie poolt saatva objekti tüüp), et saaksime teid paremini aidata.</span><span class="sxs-lookup"><span data-stu-id="8ff0b-110">If you need additional help, please open a support ticket and specify the scope of the issue (includidng the type of object you're sending to) so we can assist you better.</span></span>