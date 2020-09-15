---
title: AntiSpam 5.4.1 DBEB Catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717357"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="19463-102">Kohaletoimetamisega seotud probleemide lahendamine tõrkekood 550 5.4.1 relee juurdepääs on keelatud</span><span class="sxs-lookup"><span data-stu-id="19463-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="19463-103">See probleem ilmneb siis [, kui kontrollitakse, kas e-posti aadress kehtib bouncebacks takistamiseks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) Microsofti võrku sisenemisel.</span><span class="sxs-lookup"><span data-stu-id="19463-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="19463-104">Proovige teha järgmist.</span><span class="sxs-lookup"><span data-stu-id="19463-104">Try the following:</span></span>

1. <span data-ttu-id="19463-105">Määratlege, kas probleem on seotud kogu domeeni või ühe meiliaadressiga.</span><span class="sxs-lookup"><span data-stu-id="19463-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="19463-106">Kogu Domeen: mõnikord peab domeeni sünkroonima; Proovige [määrata Domeen asutusesiseseks ja seejärel tagasi autoriteetseks](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="19463-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="19463-107">Üks meiliaadress: mõnikord tuleb aadress sünkroonida; SMTP-puhverserveri aadressi muutmine ja selle uuesti muutmine võib aidata.</span><span class="sxs-lookup"><span data-stu-id="19463-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="19463-108">Määratlege, kas probleem on seotud mõne rühma või Ühiskaustaga.</span><span class="sxs-lookup"><span data-stu-id="19463-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="19463-109">Mõne objekti tüübi korral võib olla vaja, et Azure Active Directorys on objektid käsitsi loodud.</span><span class="sxs-lookup"><span data-stu-id="19463-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="19463-110">Kui vajate täiendavat abi, avage klienditoe pilet ja määrake probleemi ulatus (sh objekti tüüp), et saaksime teid paremini aidata.</span><span class="sxs-lookup"><span data-stu-id="19463-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>