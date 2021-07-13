---
title: Väljaminevate kattekaustade
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381633"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="f53d2-102">Väljaminevate kattekaustade</span><span class="sxs-lookup"><span data-stu-id="f53d2-102">Outbound relay pool</span></span>

<span data-ttu-id="f53d2-103">Microsoft muudab konfiguratsiooni meilisõnumite edastamiseks või edasisaatmiseks Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f53d2-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="f53d2-104">Teatud stsenaariumides sõnumeid edastatakse või edastatakse Microsoft 365 kaudu, kasutades spetsiaalset releekausta.</span><span class="sxs-lookup"><span data-stu-id="f53d2-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="f53d2-105">Releekausta abil saadetud sõnumid võivad olla adressaadi rämpspostikaustas.</span><span class="sxs-lookup"><span data-stu-id="f53d2-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="f53d2-106">Lisateavet leiate teemast [Väljaminevate tarnete kaustu](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="f53d2-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="f53d2-107">Releekausta kasutamise vältimiseks veenduge, et edasi saadetud/edastatud sõnumid vastaksid ühele järgmistest kriteeriumidest.</span><span class="sxs-lookup"><span data-stu-id="f53d2-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="f53d2-108">Väljamineva saatja on rentniku aktsepteeritud domeen.</span><span class="sxs-lookup"><span data-stu-id="f53d2-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="f53d2-109">Saatjapoliitika raamistik (SPF) möödub, kui sõnum jõuab Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f53d2-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="f53d2-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f53d2-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="f53d2-111">Ülaltoodud kriteeriumidele vastavad sõnumid ei edastata releekausta kaudu.</span><span class="sxs-lookup"><span data-stu-id="f53d2-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="f53d2-112">Kui teie domeeni MX-kirje on suunatud kolmandale osapoolele või asutusesisesele serverile, kasutage täiustatud filtreerimist, et veenduda, kas SPF-i valideerimine on sissetulevate meilisõnumite jaoks õige ja et vältida meilisõnumite saatmist läbi releekausta.</span><span class="sxs-lookup"><span data-stu-id="f53d2-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="f53d2-113">**Kuidas saame teada, kas me oleme releekausta mõjul?**</span><span class="sxs-lookup"><span data-stu-id="f53d2-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="f53d2-114">Kui teie edastatud või edastatud meilisõnumid kasutavad ühte ülaltoodud kriteeriumidest, ei edastata sõnumeid läbi releekausta.</span><span class="sxs-lookup"><span data-stu-id="f53d2-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="f53d2-115">Kui aga sõnum saadetakse releekausta kaudu, on väljamineva meili serveri IP vahemikus 40.95.0.0/16 ja väljamineva meili serveri nimi **sisaldab nime rly.**</span><span class="sxs-lookup"><span data-stu-id="f53d2-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

