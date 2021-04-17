---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821443"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="d470e-102">Tõrkekoodi 550 5.4.1 edastamisega seotud probleemide lahendamine</span><span class="sxs-lookup"><span data-stu-id="d470e-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="d470e-103">See probleem ilmneb [siis, kui kontrollite, kas](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) meiliaadress on kehtiv, et vältida Microsofti võrku sisenemisel tagasipöördumiseid.</span><span class="sxs-lookup"><span data-stu-id="d470e-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="d470e-104">Proovige järgmist.</span><span class="sxs-lookup"><span data-stu-id="d470e-104">Try the following:</span></span>

1. <span data-ttu-id="d470e-105">Tehke kindlaks, kas probleem on seotud terve domeeni või ühe meiliaadressiga.</span><span class="sxs-lookup"><span data-stu-id="d470e-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="d470e-106">Kogu domeen. Mõnikord tuleb domeen sünkroonida; proovige [määrata domeeniks Internal (Sisemine) ja seejärel valige uuesti Authoritative (Autoriteetne).](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)</span><span class="sxs-lookup"><span data-stu-id="d470e-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="d470e-107">Ühekordne meiliaadress: mõnikord tuleb aadress sünkroonida; Smtp-puhverserveri aadressi muutmine ja selle tagasi muutmine võib aidata.</span><span class="sxs-lookup"><span data-stu-id="d470e-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="d470e-108">Tehke kindlaks, kas probleem on seotud rühma või avaliku kaustaga.</span><span class="sxs-lookup"><span data-stu-id="d470e-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="d470e-109">Mõne objektitüübi puhul tuleb objektid azure Active Directorys käsitsi luua.</span><span class="sxs-lookup"><span data-stu-id="d470e-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="d470e-110">Kui vajate täiendavat abi, avage tugiteenuste pilet ja määrake probleemi ulatus (sh selle objekti tüüp, mida saadate), et saaksime teid paremini aidata.</span><span class="sxs-lookup"><span data-stu-id="d470e-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>